---
title: "IRepD2ShapeObjFilledAreaInt.YChannelDifferential"
description: "Specifies the y1-channel of a curve in the Filled area display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjFilledAreaInt.YChannelDifferential

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannelDifferential for 2DFilledArea

Specifies the y1-channel of a curve in the Filled area display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.YChannelDifferential
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMyShape.Settings.FillEffects.Color.ColorIndex = dd.eColorIndexBlue
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannelDifferential_IRepD2ShapeObjFilledAreaInt.htm`*

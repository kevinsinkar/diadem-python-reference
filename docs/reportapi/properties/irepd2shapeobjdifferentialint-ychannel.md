---
title: "IRepD2ShapeObjDifferentialInt.YChannel"
description: "Specifies the y-channel of a curve in the Differential display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjDifferentialInt.YChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannel for 2DDifferential

Specifies the y-channel of a curve in the Differential display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.YChannel
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeDifferential, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Type = dd.e2DDifferentialRange
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.BorderLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannel_IRepD2ShapeObjDifferentialInt.htm`*

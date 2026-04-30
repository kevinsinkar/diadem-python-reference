---
title: "IRepD2ShapeObjBarsInt.XChannel"
description: "Specifies the x-channel of a curve in the Bars display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjBarsInt.XChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XChannel for 2DBars

Specifies the x-channel of a curve in the Bars display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.XChannel
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[2]"
oMySettings = oMyShape.Settings
oMySettings.Filling.Pattern = dd.eFillPatternFilled
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexTurquoise)
oMySettings.Width = 50
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XChannel_IRepD2ShapeObjBarsInt.htm`*

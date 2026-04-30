---
title: "IRepD2BarFillingInt.UseSameColorAsBorder"
description: "Specifies whether DIAdem REPORT displays the bar filling of a 2D axis system in the same color as the curve."
---

# IRepD2BarFillingInt.UseSameColorAsBorder

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseSameColorAsBorder for 2DBarFilling

Specifies whether DIAdem REPORT displays the bar filling of a 2D axis system in the same color as the curve.

## Signature

```python
obj.UseSameColorAsBorder
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFilling = oMySettings.Filling
oMyFilling.UseSameColorAsBorder = False
oMyFilling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyFilling.Pattern = dd.eFillPatternCrossDiagonal
oMyFilling.Density = 30
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseSameColorAsBorder_IRepD2BarFillingInt.htm`*

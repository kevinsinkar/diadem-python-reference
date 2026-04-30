---
title: "IRepD2BarFillingInt.Color"
description: "Specifies the color of a bar display in a 2D axis system in DIAdem REPORT. DIAdem only includes the property Color if you assign the value FALSE to the UseSameC"
---

# IRepD2BarFillingInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for 2DBarFilling

Specifies the color of a bar display in a 2D axis system in DIAdem REPORT. DIAdem only includes the property Color if you assign the value FALSE to the UseSameColorAsBorder property.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexNone)
oMyFilling = oMySettings.Filling
oMyFilling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyFilling.Pattern = dd.eFillPatternCrossDiagonal
oMyFilling.Density = 30
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepD2BarFillingInt.htm`*

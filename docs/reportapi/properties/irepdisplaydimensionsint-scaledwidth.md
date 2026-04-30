---
title: "IRepDisplayDimensionsInt.ScaledWidth"
description: "Specifies the page width of worksheets in DIAdem REPORT, in centimeters or inches. DIAdem only includes the ScaledWidth property if you assign the value TRUE to"
---

# IRepDisplayDimensionsInt.ScaledWidth

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ScaledWidth for DisplayDimensions

Specifies the page width of worksheets in DIAdem REPORT, in centimeters or inches. DIAdem only includes the ScaledWidth property if you assign the value TRUE to the UseScaledOutput property.

## Signature

```python
obj.ScaledWidth
```

## Python example

```python
dd.Report.NewLayout()
dd.Report.Settings.Page.Dimensions.UseScaledOutput = True
dd.Report.Settings.Page.Dimensions.ScaledHeight = 26
dd.Report.Settings.Page.Dimensions.ScaledWidth = 18
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 2
oMyPos.X2 = 15
oMyPos.Y1 = 5
oMyPos.Y2 = 15
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ScaledWidth_IRepDisplayDimensionsInt.htm`*

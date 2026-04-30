---
title: "IRepDisplayDimensionsInt.UseScaledOutput"
description: "Specifies whether DIAdem REPORT enables scaled display."
---

# IRepDisplayDimensionsInt.UseScaledOutput

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseScaledOutput for DisplayDimensions

Specifies whether DIAdem REPORT enables scaled display.

## Signature

```python
obj.UseScaledOutput
```

## Python example

```python
dd.Report.NewLayout()
oMyPageDimensions = dd.Report.Settings.Page.Dimensions
oMyPageDimensions.UseScaledOutput = True
oMyPageDimensions.ScaledHeight = 26
oMyPageDimensions.ScaledWidth = 18
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 2
oMyPos.X2 = 15
oMyPos.Y1 = 5
oMyPos.Y2 = 15
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyXScaling = oMy2DAxisSystem.XAxis.Scaling.ScaledOutput
oMyXScaling.AutoScalingType = dd.eAxisAutoScalingScaledOutputCompleteAutomatic
oMyYScaling = oMy2DAxisSystem.YAxis.Scaling.ScaledOutput
oMyYScaling.AutoScalingType = dd.eAxisAutoScalingScaledOutputCompleteAutomatic
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseScaledOutput_IRepDisplayDimensionsInt.htm`*

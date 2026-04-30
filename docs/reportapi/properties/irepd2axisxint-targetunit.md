---
title: "IRepD2AxisXInt.TargetUnit"
description: "Specifies the unit for the values of the x-axis in a 2D axis system in DIAdem REPORT. If you assign a value to the property TargetUnit , DIAdem converts the cha"
---

# IRepD2AxisXInt.TargetUnit

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TargetUnit for 2DAxisX

Specifies the unit for the values of the x-axis in a 2D axis system in DIAdem REPORT. If you assign a value to the property TargetUnit , DIAdem converts the channels you want to display into this unit. If DIAdem cannot convert the unit, DIAdem does not display the data.

## Signature

```python
obj.TargetUnit
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
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.TargetUnit = "min"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TargetUnit_IRepD2AxisXInt.htm`*

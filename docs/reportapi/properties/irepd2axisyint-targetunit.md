---
title: "IRepD2AxisYInt.TargetUnit"
description: "Specifies the unit for the values of the y-axis in a 2D axis system in DIAdem REPORT. If you assign a value to the property TargetUnit , DIAdem converts the cha"
---

# IRepD2AxisYInt.TargetUnit

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TargetUnit for 2DAxisY

Specifies the unit for the values of the y-axis in a 2D axis system in DIAdem REPORT. If you assign a value to the property TargetUnit , DIAdem converts the channels you want to display into this unit. If DIAdem cannot convert the unit, DIAdem does not display the data.

## Signature

```python
obj.TargetUnit
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.TargetUnit = "h"
oMy2DAxisSystem.YAxis.TargetUnit = "km/h"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TargetUnit_IRepD2AxisYInt.htm`*

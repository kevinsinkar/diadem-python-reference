---
title: "IRepAxisTickInt.Distance"
description: "Specifies the interval between the ticks you want labeled in units of the axis range, in a 3D axis system or in polar axis system in DIAdem REPORT. If the scali"
---

# IRepAxisTickInt.Distance

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Distance for AxisTickObject

Specifies the interval between the ticks you want labeled in units of the axis range, in a 3D axis system or in polar axis system in DIAdem REPORT. If the scaling is not logarithmic, the value of the Distance property is the space between the main ticks you want to label. If the scaling is logarithmic, DIAdem interprets the values before the decimal point and the values after the decimal point of the Distance property separately. The integer value before the decimal point specifies the steps between two labels, which are powers of ten. For example, if the axis origin and the tick interval have the value 1, DIAdem labels the ticks at 10 0 , 10 1 , 10 2 and so on. For example, if you assign the value 3 to the tick interval, DIAdem labels the ticks at 10 0 , 10 3 , 10 6 and so on. The reciprocal value after the decimal point, specifies intervals that you want to label in the ranges defined by the value before the decimal point. For example, if you assign the value 1.25 to the Distance property, DIAdem divides the area into quarters.

## Signature

```python
obj.Distance
```

## Python example

```python
dd.Report.NewLayout()
oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem, "My3DAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMyAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyXScaling = oMyAxisSystem.AxisList.X.Scaling
oMyXScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyXScaling.Tick.SpacingType = dd.eAxisTickSpacingDefinedByDistance
oMyXScaling.Tick.Distance = 0.5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Distance_IRepAxisTickInt.htm`*

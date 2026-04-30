---
title: "IRepAxisTickInt.SpacingType"
description: "Specifies whether DIAdem REPORT takes the tick positions in an axis system from a data channel or calculates the tick positions automatically."
---

# IRepAxisTickInt.SpacingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SpacingType for AxisTickObject

Specifies whether DIAdem REPORT takes the tick positions in an axis system from a data channel or calculates the tick positions automatically.

## Signature

```python
obj.SpacingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisTickSpacingDefinedByDistance` | 0 | Calculated from tick distance |
| `eAxisTickSpacingReadFromChannel` | 1 | Read from tick channel |

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

*Source: `ReportApi/properties/Report_property_SpacingType_IRepAxisTickInt.htm`*

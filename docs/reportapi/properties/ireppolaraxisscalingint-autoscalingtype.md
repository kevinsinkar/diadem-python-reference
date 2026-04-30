---
title: "IRepPolarAxisScalingInt.AutoScalingType"
description: "Specifies whether DIAdem scales the radial axis of the polar axis system automatically."
---

# IRepPolarAxisScalingInt.AutoScalingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AutoScalingType for PolarAxisScaling

Specifies whether DIAdem scales the radial axis of the polar axis system automatically.

## Signature

```python
obj.AutoScalingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisScalingSimpleManual` | 0 | Manual |
| `eAxisScalingSimpleCompleteAutomatic` | 1 | Fully automatic |
| `eAxisAutoScalingCustom` | 2 | User-defined axis scaling |

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyScaling = oMyPolarAxisSystem.RadialAxis.Scaling
oMyScaling.Type = dd.ePolarScalingLinear
oMyScaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyScaling.Begin = 10
oMyScaling.End = 20
oMyScaling.Origin = 5
oMyScaling.Tick.Distance = 5
oMyScaling.MiniTickCount = 2
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AutoScalingType_IRepPolarAxisScalingInt.htm`*

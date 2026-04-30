---
title: "IRepPolarAxisScalingInt.Tick"
description: "Specifies the properties of the radial axis ticks in a polar axis system in DIAdem REPORT."
---

# IRepPolarAxisScalingInt.Tick

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Tick for PolarAxisScaling

Specifies the properties of the radial axis ticks in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Tick
```

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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Tick_IRepPolarAxisScalingInt.htm`*

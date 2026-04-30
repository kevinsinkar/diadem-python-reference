---
title: "IRepPolarAxisScalingInt.Origin"
description: "Specifies from which value DIAdem starts labeling the radial axis of the polar axis system in DIAdem REPORT. DIAdem only includes the property Origin if you ass"
---

# IRepPolarAxisScalingInt.Origin

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Origin for PolarAxisScaling

Specifies from which value DIAdem starts labeling the radial axis of the polar axis system in DIAdem REPORT. DIAdem only includes the property Origin if you assign the value eAxisScalingSimpleManual to the AutoScalingType property.

## Signature

```python
obj.Origin
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

*Source: `ReportApi/properties/Report_property_Origin_IRepPolarAxisScalingInt.htm`*

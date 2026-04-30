---
title: "IRepPolarInt.RadialAxis"
description: "Specifies the properties of a radial axis in a polar axis system in DIAdem REPORT."
---

# IRepPolarInt.RadialAxis

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RadialAxis for PolarSystem

Specifies the properties of a radial axis in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.RadialAxis
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.RadialAxis.Scaling.Begin = 10
oMyPolarAxisSystem.RadialAxis.Scaling.End = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RadialAxis_IRepPolarInt.htm`*

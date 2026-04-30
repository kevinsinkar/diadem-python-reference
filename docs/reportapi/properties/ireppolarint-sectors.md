---
title: "IRepPolarInt.Sectors"
description: "Returns a collection of all sectors in a polar axis system in DIAdem REPORT."
---

# IRepPolarInt.Sectors

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Sectors for PolarSystem

Returns a collection of all sectors in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Sectors
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.Sectors.SectorLine.LineType = dd.eLineTypeDashed1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Sectors_IRepPolarInt.htm`*

---
title: "IRepReportMasterLayoutInt.IsUpdateRequired"
description: "Checks whether the master layout in DIAdem REPORT needs to be refreshed."
---

# IRepReportMasterLayoutInt.IsUpdateRequired

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: IsUpdateRequired for MasterLayout

Checks whether the master layout in DIAdem REPORT needs to be refreshed.

## Signature

```python
bIsUpdateRequired = Object.IsUpdateRequired()
```

## Python example

```python
if dd.Report.Settings.MasterLayout.IsUpdateRequired :
    dd.Report.Settings.MasterLayout.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_IsUpdateRequired_IRepReportMasterLayoutInt.htm`*

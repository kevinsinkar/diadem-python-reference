---
title: "IRepPolarInt.Settings"
description: "Specifies the properties of a polar axis system in DIAdem REPORT."
---

# IRepPolarInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for PolarSystem

Specifies the properties of a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepPolarInt.htm`*

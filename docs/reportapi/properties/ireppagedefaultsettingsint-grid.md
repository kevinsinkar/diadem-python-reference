---
title: "IRepPageDefaultSettingsInt.Grid"
description: "Specifies the background grid of a worksheet in DIAdem REPORT."
---

# IRepPageDefaultSettingsInt.Grid

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Grid for PageDefaultSettings

Specifies the background grid of a worksheet in DIAdem REPORT.

## Signature

```python
return_value = obj.Grid
```

## Python example

```python
oMyPageGridSettings = dd.Report.Settings.Page.Grid
oMyPageGridSettings.Enable = True
oMyPageGridSettings.Spacing = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Grid_IRepPageDefaultSettingsInt.htm`*

---
title: "IRepPageGridInt.Enable"
description: "Specifies whether DIAdem REPORT displays a grid in the background."
---

# IRepPageGridInt.Enable

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Enable for PageGridSettings

Specifies whether DIAdem REPORT displays a grid in the background.

## Signature

```python
obj.Enable
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
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Enable_IRepPageGridInt.htm`*

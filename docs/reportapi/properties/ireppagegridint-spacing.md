---
title: "IRepPageGridInt.Spacing"
description: "Specifies the spaces between the grid lines as a percentage of the worksheet in cm or inch, in DIAdem REPORT. Enable the grid with the property Enable ."
---

# IRepPageGridInt.Spacing

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Spacing for PageGridSettings

Specifies the spaces between the grid lines as a percentage of the worksheet in cm or inch, in DIAdem REPORT. Enable the grid with the property Enable .

## Signature

```python
obj.Spacing
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

*Source: `ReportApi/properties/Report_property_Spacing_IRepPageGridInt.htm`*

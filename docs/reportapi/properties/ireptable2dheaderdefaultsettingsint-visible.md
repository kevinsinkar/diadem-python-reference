---
title: "IRepTable2DHeaderDefaultSettingsInt.Visible"
description: "Specifies whether DIAdem REPORT displays headers and footers of a 2D table. You can specify the height of the headers and footers with the Height property."
---

# IRepTable2DHeaderDefaultSettingsInt.Visible

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Visible for 2DTableHeaderFooterDefaultSettings

Specifies whether DIAdem REPORT displays headers and footers of a 2D table. You can specify the height of the headers and footers with the Height property.

## Signature

```python
obj.Visible
```

## Python example

```python
o2DTableHeaderFooterDefaultSettings = dd.Report.ActiveSheet.Objects("2D-Table").Settings.Footer
o2DTableHeaderFooterDefaultSettings.Visible = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Visible_IRepTable2DHeaderDefaultSettingsInt.htm`*

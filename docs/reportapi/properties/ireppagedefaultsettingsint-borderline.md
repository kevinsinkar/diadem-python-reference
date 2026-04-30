---
title: "IRepPageDefaultSettingsInt.BorderLine"
description: "Specifies the display of the global frame line of a worksheet in DIAdem REPORT."
---

# IRepPageDefaultSettingsInt.BorderLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BorderLine for PageDefaultSettings

Specifies the display of the global frame line of a worksheet in DIAdem REPORT.

## Signature

```python
return_value = obj.BorderLine
```

## Python example

```python
dd.Report.NewLayout()
oMyBorderLine = dd.Report.Settings.Page.BorderLine
oMyBorderLine.Color.SetPredefinedColor(dd.ePredefinedColorDarkViolet)
oMyBorderLine.Width = dd.eLineWidth0800
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BorderLine_IRepPageDefaultSettingsInt.htm`*

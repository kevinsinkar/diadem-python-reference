---
title: "IRepSettingsInt.DefaultFontType"
description: "Specifies the font for all texts and numbers to which you did not assign a specific font in DIAdem REPORT."
---

# IRepSettingsInt.DefaultFontType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DefaultFontType for Settings

Specifies the font for all texts and numbers to which you did not assign a specific font in DIAdem REPORT.

## Signature

```python
obj.DefaultFontType
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note </strong>  Use the properties <span class="Monospace">eDefaultFontTypeSystem</span> or <span class="Monospace">eDefaultFontTypeWindows</span> to read the report worldwide, regardless of the interface language of your operating system.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDefaultFontTypeOwn` | 0 | Use this setting to display a report on different computers in the same font. Specify the font with the DefaultFontName property. The selected font must be on all computers so that DIAdem displays the report identically. |
| `eDefaultFontTypeSystem` | 1 | DIAdem uses the default font of your operating system for all texts and numbers in a report to which you did not assign a specific font. |
| `eDefaultFontTypeWindows` | 2 | DIAdem uses the default font of your operating system for all texts and numbers in a report to which you did not assign a specific font. |

## Python example

```python
dd.Report.Settings.DefaultFontType = dd.eDefaultFontTypeOwn
dd.Report.Settings.DefaultFontName = "Times Roman"()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DefaultFontType_IRepSettingsInt.htm`*

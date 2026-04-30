---
title: "IRepSettingsInt.DefaultFontName"
description: "Specifies, in DIAdem REPORT, the font name for all texts and numbers to which you did not explicitly assign a different font. You must assign the value eDefault"
---

# IRepSettingsInt.DefaultFontName

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DefaultFontName for Settings

Specifies, in DIAdem REPORT, the font name for all texts and numbers to which you did not explicitly assign a different font. You must assign the value eDefaultFontTypeOwn to the DefaultFontType property for DIAdem to use the specified font in the DefaultFontName property.

## Signature

```python
obj.DefaultFontName
```

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

*Source: `ReportApi/properties/Report_property_DefaultFontName_IRepSettingsInt.htm`*

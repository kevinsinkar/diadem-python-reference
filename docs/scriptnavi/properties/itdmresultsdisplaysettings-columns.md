---
title: "ITDMResultsDisplaySettings.Columns"
description: "Specifies in a search in DIAdem NAVIGATOR the property columns to be displayed for the different result types."
---

# ITDMResultsDisplaySettings.Columns

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Columns for ResultsListSettings

Specifies in a search in DIAdem NAVIGATOR the property columns to be displayed for the different result types.

## Signature

```python
return_value = obj.Columns
```

## Python example

```python
oMySettings = dd.Navigator.Display.CurrDataFinder.ResultsList.Settings
dd.MsgBoxDisp(oMySettings.Columns(dd.eSearchFile).Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Columns_ITDMResultsDisplaySettings.htm`*

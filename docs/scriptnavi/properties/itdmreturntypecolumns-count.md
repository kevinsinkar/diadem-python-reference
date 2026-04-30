---
title: "ITDMReturnTypeColumns.Count"
description: "Determines the number of columns that DIAdem-NAVIGATOR displays in the search result list of a search in a data store."
---

# ITDMReturnTypeColumns.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for ReturnTypeColumns

Determines the number of columns that DIAdem-NAVIGATOR displays in the search result list of a search in a data store.

## Signature

```python
obj.Count
```

## Python example

```python
oMyReturnTypeColumn = dd.Navigator.Display.CurrDataStore.ResultsList.Settings.Columns
print (oMyReturnTypeColumn.Item("aotest").Count)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMReturnTypeColumns.htm`*

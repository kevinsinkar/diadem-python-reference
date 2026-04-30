---
title: "IDataStoreCell.Column"
description: "Specifies in the search results list of a data store a column with properties."
---

# IDataStoreCell.Column

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Column for Cell <DataStore>

Specifies in the search results list of a data store a column with properties.

## Signature

```python
return_value = obj.Column
```

## Python example

```python
oMyResultsList = dd.Navigator.Display.CurrDataStore.ResultsList
oMyCell = oMyResultsList.FocusedCell
dd.MsgBoxDisp(oMyCell.Column.Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Column_IDataStoreCell.htm`*

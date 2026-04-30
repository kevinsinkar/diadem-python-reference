---
title: "IDataStoreCell.Element"
description: "Returns the element which is associated to a cell, in the search results list of a data store."
---

# IDataStoreCell.Element

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Element for Cell <DataStore>

Returns the element which is associated to a cell, in the search results list of a data store.

## Signature

```python
return_value = obj.Element
```

## Python example

```python
oMyResultsList = dd.Navigator.Display.CurrDataStore.ResultsList
oMyCell = oMyResultsList.FocusedCell
dd.MsgBoxDisp(oMyCell.Element.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Element_IDataStoreCell.htm`*

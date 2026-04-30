---
title: "INaviDataStoreResultDisplay.Selection"
description: "Specifies the elements, cells, or columns currently selected in the search results list of a data store."
---

# INaviDataStoreResultDisplay.Selection

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Selection for ResultsList <DataStore>

Specifies the elements, cells, or columns currently selected in the search results list of a data store.

## Signature

```python
return_value = obj.Selection
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The properties <a href="../inavidatastoreresultdisplay-cellsselection/">CellsSelection</a>, <a href="../inavidatastoreresultdisplay-columnsselection/">ColumnsSelection</a>, and <a href="../inavidatastoreresultdisplay-elementsselection/">ElementsSelection</a> contain the specific type of an element selected in the search results.</td></tr></table>
</div>

## Python example

```python
dd.Navigator.LoadData(Navigator.Display.CurrDataStore.ResultsList.Selection)
```

---

*Source: `ScriptNavi/properties/navigator_property_Selection_INaviDataStoreResultDisplay.htm`*

---
title: "ITDMResultsDisplayCellsSelection.IsKindOf"
description: "Specifies the type of an element selected in the search results list of a DataFinder or of a data store."
---

# ITDMResultsDisplayCellsSelection.IsKindOf

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsKindOf for CellsSelection

Specifies the type of an element selected in the search results list of a DataFinder or of a data store.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColumnsSelection` | 1 | Column ( Column (ColumnsSelection ) |
| `eElementsSelection` | 2 | Element ( ElementsSelection <DataFinder> , ElementsSelection <DataStore> ) |
| `eCellsSelection` | 4 | Cell ( CellsSelection ) |

## Python example

```python
oMyResultsListSelection=dd.Navigator.Display.CurrDataStore.ResultsList.Selection
if oMyResultsListSelection.IsKindOf(dd.eElementsSelection) :
    dd.MsgBoxDisp(oMyResultsListSelection.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsKindOf_ITDMResultsDisplayCellsSelection.htm`*

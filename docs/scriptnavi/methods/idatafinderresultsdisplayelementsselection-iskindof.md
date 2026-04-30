---
title: "IDataFinderResultsDisplayElementsSelection.IsKindOf"
description: "Determines whether you selected elements, cells, or columns in the search results of a DataFinder."
---

# IDataFinderResultsDisplayElementsSelection.IsKindOf

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsKindOf for ElementsSelection <DataFinder>

Determines whether you selected elements, cells, or columns in the search results of a DataFinder.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColumnsSelection` | 1 | Column ( Column (ColumnsSelection ) |
| `eElementsSelection` | 2 | Element ( ElementsSelection <DataFinder> ) |
| `eCellsSelection` | 4 | Cell ( CellsSelection ) |

## Python example

```python
oMyResultsListSelection=dd.Navigator.Display.CurrDataFinder.ResultsList.Selection
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

*Source: `ScriptNavi/methods/navigator_method_IsKindOf_IDataFinderResultsDisplayElementsSelection.htm`*

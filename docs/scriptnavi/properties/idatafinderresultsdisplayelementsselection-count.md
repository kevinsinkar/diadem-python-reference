---
title: "IDataFinderResultsDisplayElementsSelection.Count"
description: "Specifies the number of rows selected in a search results list of a DataFinder."
---

# IDataFinderResultsDisplayElementsSelection.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for ElementsSelection <DataFinder>

Specifies the number of rows selected in a search results list of a DataFinder.

## Signature

```python
obj.Count
```

## Python example

```python
ElementsSelection = dd.Navigator.Display.CurrDataFinder.ResultsList.ElementsSelection
for Index in range( 1, ElementsSelection.Count+1):
    dd.MsgBoxDisp(ElementsSelection(Index).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_IDataFinderResultsDisplayElementsSelection.htm`*

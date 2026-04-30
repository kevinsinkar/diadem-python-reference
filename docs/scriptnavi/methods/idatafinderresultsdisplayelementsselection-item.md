---
title: "IDataFinderResultsDisplayElementsSelection.Item"
description: "Returns the ElementsSelection object associated with a certain index, in the search results list of a DataFinder ."
---

# IDataFinderResultsDisplayElementsSelection.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for ElementsSelection <DataFinder>

Returns the ElementsSelection object associated with a certain index, in the search results list of a DataFinder .

## Signature

```python
return_value = obj.Item(Index)
```

## Python example

```python
ElementsSelection = dd.Navigator.Display.CurrDataFinder.ResultsList.ElementsSelection
if ElementsSelection.IsKindOf(dd.eElementsSelection) :
    Element = ElementsSelection.Item(1)
    dd.MsgBoxDisp(Element.Name)
else:
    dd.MsgBoxDisp("no element selected")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IDataFinderResultsDisplayElementsSelection.htm`*

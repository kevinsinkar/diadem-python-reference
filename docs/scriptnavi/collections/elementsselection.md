---
title: "ElementsSelection"
description: "Collection of the rows selected in the search results of a DataFinder."
---

# ElementsSelection

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ElementsSelection <DataFinder>

Collection of the rows selected in the search results of a DataFinder.

## Python example

```python
oMyCurrDataProvider = dd.Navigator.Display.CurrDataFinder
oMyQueryForm = oMyCurrDataProvider.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType = dd.eSearchFile
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add(dd.eSearchFile,"fileName","=","Brake*")
oMyQueryForm.Search()
dd.WndShow("NAVIGATOR", "SHOW")
dd.InterActionOn("Select one or more elements of the search results")
dd.WndShow("SCRIPT", "SHOW")
oMyResultsList = oMyCurrDataProvider.ResultsList
oMyElementsSelection = oMyResultsList.ElementsSelection
if oMyElementsSelection.IsKindOf(dd.eElementsSelection) :
    for Element in oMyElementsSelection:
        dd.MsgBoxDisp("Name: " + Element.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatafinderresultsdisplayelementsselection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatafinderresultsdisplayelementsselection-iskindof/">IsKindOf</a> | <a href="../../methods/idatafinderresultsdisplayelementsselection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavidatafinderresultdisplay/">ResultsList &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderresultdisplay-elementsselection/">ElementsSelection</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataFinderResultsDisplayElementsSelection.htm`*

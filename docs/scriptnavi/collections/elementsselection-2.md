---
title: "ElementsSelection"
description: "Collection of the rows selected in the search results of a data store. Only read access."
---

# ElementsSelection

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ElementsSelection <DataStore>

Collection of the rows selected in the search results of a data store. Only read access.

## Python example

```python
oMyDataStore = dd.Navigator.Display.CurrDataStore
oMyQueryForm = oMyDataStore.QueryForm
oMyQueryForm.Conditions.RemoveAll()
oMyConditions = oMyQueryForm.Conditions
oMyConditions.Add("Test","Name","=","ETC")
oMyConditions.Add("Measurement","Name","=","DL")
oMyConditions.Logic = "C1 and C2"
oMyQueryForm.Search()
oMyResultsList = oMyDataStore.ResultsList
dd.WndShow("NAVIGATOR", "SHOW")
dd.InterActionOn("Select one or more elements of the search results")
dd.WndShow("SCRIPT", "SHOW")
oMySelectedElements = oMyDataStore.ResultsList.ElementsSelection
dd.Navigator.LoadData(oMySelectedElements, "Load")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatastoreresultsdisplayelementsselection-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatastoreresultsdisplayelementsselection-iskindof/">IsKindOf</a> | <a href="../../methods/idatastoreresultsdisplayelementsselection-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/inavidatastoreresultdisplay/">ResultsList &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastoreresultdisplay-elementsselection/">ElementsSelection</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataStoreResultsDisplayElementsSelection.htm`*

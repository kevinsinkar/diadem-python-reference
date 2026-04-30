---
title: "INaviDataStoreResultDisplay.ResultsElements"
description: "Returns in an interface search of a data store a collection of the currently displayed search results."
---

# INaviDataStoreResultDisplay.ResultsElements

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsElements for ResultsList <DataStore>

Returns in an interface search of a data store a collection of the currently displayed search results.

## Signature

```python
return_value = obj.ResultsElements
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <a href="../itdmstoreelementlist-maxcount/">MaxCount</a> property specifies the maximum number of elements that a search returns to the search results. The <a href="../itdmstoreelementlist-isincomplete/">IsIncomplete</a> property specifies whether the search results contain all the search results elements.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.Display.CurrDataStore
oMyQuery = oMyDataStore.QueryForm
oMyQuery.ReturnType = "MeaQuantity"
oMyQueryForm = oMyDataStore.QueryForm
oMyQueryForm.ResultsMode = dd.eResultsModeElements

oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add("MeaQuantity","minimum","<=","20")
oMyConditions.Logic = "C1"

oMyDataStore.QueryForm.Search()
oMyResultsList = oMyDataStore.ResultsList
dd.MsgBoxDisp("Number of results: " + oMyResultsList.ResultsElements.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsElements_INaviDataStoreResultDisplay.htm`*

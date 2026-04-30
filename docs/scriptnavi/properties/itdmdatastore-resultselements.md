---
title: "ITDMDataStore.ResultsElements"
description: "Returns the search results of a search without user interface for elements in a data store."
---

# ITDMDataStore.ResultsElements

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsElements for DataStore

Returns the search results of a search without user interface for elements in a data store.

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
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")

oMyQuery = oMyDataStore.CreateQuery(dd.eDataStoreQuery)
oMyQuery.ReturnType = "measurement"
oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add("MeaQuantity","minimum",">=","900")
oMyConditions.Logic = "C1"

oMyDataStore.SearchElements(oMyQuery)
oMyResults = oMyDataStore.ResultsElements
dd.Navigator.LoadData(oMyResults,None ,None)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsElements_ITDMDataStore.htm`*

---
title: "ITDMDataStore.SearchElements"
description: "Makes an interfaceless query for elements from a data store. You must transfer the search conditions as a parameter. Use the SearchElements method to execute a "
---

# ITDMDataStore.SearchElements

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SearchElements for DataStore

Makes an interfaceless query for elements from a data store. You must transfer the search conditions as a parameter. Use the SearchElements method to execute a Quick search and an Advanced search . Use the ResultsElements property to access the search results.

## Signature

```python
obj.SearchElements(Query, [MaxCount])
```

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
dd.Navigator.LoadData(oMyResults, "Load", None)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SearchElements_ITDMDataStore.htm`*

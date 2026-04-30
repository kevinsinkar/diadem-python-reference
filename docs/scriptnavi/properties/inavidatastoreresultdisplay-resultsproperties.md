---
title: "INaviDataStoreResultDisplay.ResultsProperties"
description: "Specifies the search result of a column-oriented interface search in a data store. If you search for elements ( ResultsMode = eResultsModeElements) , DIAdem ret"
---

# INaviDataStoreResultDisplay.ResultsProperties

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsProperties for ResultsList <DataStore>

Specifies the search result of a column-oriented interface search in a data store. If you search for elements ( ResultsMode = eResultsModeElements) , DIAdem returns the search results in the property ResultsList . ResultsElements . If you execute a column oriented search ( ResultsMode = eResultsModeProperties ), DIAdem returns the search results in the property ResultsList . ResultsProperties .

## Signature

```python
return_value = obj.ResultsProperties
```

## Python example

```python
oMyDataStore = dd.Navigator.Display.CurrDataStore
oMyQuery = oMyDataStore.QueryForm
oMyQuery.ReturnType = "measurement"
oMyQueryForm = oMyDataStore.QueryForm
oMyQueryForm.ResultsMode = dd.eResultsModeProperties

oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add("measurement","minimum","<=","20")
oMyConditions.Logic = "C1"
#Define Result Columns
oMyResultsColumns = oMyDataStore.ResultsList.Settings.Columns
oMyResultsColumn = oMyResultsColumns("meaquantity")
#Fill Results Columns
oMyResultsColumn.RemoveAll()
oMyResultsColumn.Add("measurement","name")
oMyResultsColumn.Add("measurement", "ID")
#Search
oMyDataStore.QueryForm.Search()
oMyResults = oMyDataStore.ResultsList.ResultsProperties
dd.MsgBoxDisp(oMyResults.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsProperties_INaviDataStoreResultDisplay.htm`*

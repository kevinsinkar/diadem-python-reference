---
title: "ITDMDataStore.ResultsProperties"
description: "Returns the results of a column-oriented search without the user interface in a data store."
---

# ITDMDataStore.ResultsProperties

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsProperties for DataStore

Returns the results of a column-oriented search without the user interface in a data store.

## Signature

```python
return_value = obj.ResultsProperties
```

## Python example

```python
dd.Data.Root.Clear()

oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyQuery = oMyDataStore.CreateQuery(dd.eDataStoreQuery)
oMyQuery.ReturnType = "measurement"
oMyConditions = oMyQuery.Conditions
oMyConditions.Add("measurement","name","=","QT_32*")
oMyConditions.Logic = "C1"

oMyResultsColumns = oMyDataStore.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add("measurement","name")
oMyResultsColumns.Add("measurement","ID")

oMyDataStore.SearchProperties(oMyQuery, oMyResultsColumns, 200)
oMyResults = oMyDataStore.ResultsProperties

dd.Navigator.LoadProperty(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsProperties_ITDMDataStore.htm`*

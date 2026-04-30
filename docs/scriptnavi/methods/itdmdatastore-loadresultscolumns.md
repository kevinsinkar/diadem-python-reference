---
title: "ITDMDataStore.LoadResultsColumns"
description: "Loads the definition of the properties columns for the search results list from a TDQ file in a data store. If the TDQ file only contains a query and no column "
---

# ITDMDataStore.LoadResultsColumns

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadResultsColumns for DataStore

Loads the definition of the properties columns for the search results list from a TDQ file in a data store. If the TDQ file only contains a query and no column configuration, the column configuration of the search results list remains unchanged and DIAdem outputs an error message. If the TDQ file contains a query and a column definition, DIAdem replaces the column configuration of the search results list with the loaded configuration. DIAdem uses the information in the TDQ file to determine the return type and loads the respective columns. If the TDQ file does not contain any information on the data type of the searched for property, DIAdem sets the data type to eNoType . In this case, change the data type manually.

## Signature

```python
return_value = obj.LoadResultsColumns(FileName)
```

## Python example

```python
#Creating a tdq file with result columns
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

oMyDataStore.SaveQuery(dd.ConfWritePath + "MyNewQuery.tdq", oMyQuery, oMyResultsColumns)
oMyResultsColumns = oMyDataStore.LoadResultsColumns(dd.ConfWritePath + "MyNewQuery.tdq")
oMyQuery = oMyDataStore.LoadQuery(dd.ConfWritePath + "MyNewQuery.tdq")
oMyDataStore.SearchProperties(oMyQuery, oMyResultsColumns, 100)
oMyResults = oMyDataStore.ResultsProperties
dd.Navigator.LoadProperty(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadResultsColumns_ITDMDataStore.htm`*

---
title: "ITDMDataFinder.LoadResultsColumns"
description: "Loads the definition of the properties columns for the search results list from a TDQ file in a DataFinder. If the TDQ file only contains a query and no column "
---

# ITDMDataFinder.LoadResultsColumns

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: LoadResultsColumns for DataFinder

Loads the definition of the properties columns for the search results list from a TDQ file in a DataFinder. If the TDQ file only contains a query and no column configuration, the column configuration of the search results list remains unchanged and DIAdem outputs an error message. If the TDQ file contains a query and a column definition, DIAdem replaces the column configuration of the search results list with the loaded configuration. DIAdem uses the information in the TDQ file to determine the return type and loads the respective columns. If the TDQ file does not contain any information on the data type of the searched for property, DIAdem sets the data type to eNoType . In this case, change the data type manually. Note Use the LoadQueryInfoSet method instead of the LoadQuery method if you want to work on the NAVIGATOR interface. Use the LoadQueryInfoSet method to also load the configuration of the search results list.

## Signature

```python
return_value = obj.LoadResultsColumns(FileName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="../idatafinderdisplay-loadqueryinfoset/">LoadQueryInfoSet</a> method instead of the <span class="Monospace">LoadQuery</span> method if you want to work on the NAVIGATOR interface. Use the <span class="Monospace">LoadQueryInfoSet</span> method to also load the configuration of the search results list.</td></tr></table>
</div>

## Python example

```python
#Creating a tdq file with result columns
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchFile

oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchChannel,"maximum","<",10)
oMyConditions.Add(dd.eSearchChannel,"minimum",">",6)
oMyConditions.Logic = "C1 and C2"

oMyResultsColumns = oMyDataFinder.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add(dd.eSearchChannel, "maximum")
oMyResultsColumns.Add(dd.eSearchChannel, "minimum")

oMyDataFinder.SaveQuery(dd.ConfWritePath + "MyNewQuery.tdq", oMyQuery, oMyResultsColumns)
```

```python
#Using the saved tdq file/result columns
oMyResultsColumns = oMyDataFinder.LoadResultsColumns(dd.ConfWritePath + "MyNewQuery.tdq")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfWritePath + "MyNewQuery.tdq")
oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumns, 100)
oMyResults = oMyDataFinder.ResultsProperties
dd.Navigator.LoadProperty(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_LoadResultsColumns_ITDMDataFinder.htm`*

---
title: "ITDMDataFinder.CreateResultsColumns"
description: "Creates an object for the definition of the results columns in a column-oriented search without user interface, in a DataFinder."
---

# ITDMDataFinder.CreateResultsColumns

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateResultsColumns for DataFinder

Creates an object for the definition of the results columns in a column-oriented search without user interface, in a DataFinder.

## Signature

```python
return_value = obj.CreateResultsColumns()
```

## Python example

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchChannel,"maximum","<=","10")
oMyConditions.Logic = "C1"

oMyResultsColumns = oMyDataFinder.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumns.Add(dd.eSearchFile, "fileName")
oMyResultsColumns.Add(dd.eSearchFile, "folder")
oMyResultsColumns.Add(dd.eSearchChannel, "maximum")

oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumns, 200)
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

*Source: `ScriptNavi/methods/navigator_method_CreateResultsColumns_ITDMDataFinder.htm`*

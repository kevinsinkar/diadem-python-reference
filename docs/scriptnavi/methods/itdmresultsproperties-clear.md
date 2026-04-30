---
title: "ITDMResultsProperties.Clear"
description: "Deletes all search results from the search results list in a column-oriented search."
---

# ITDMResultsProperties.Clear

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Clear for ResultsProperties

Deletes all search results from the search results list in a column-oriented search.

## Signature

```python
obj.Clear()
```

## Python example

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.Add(dd.eSearchChannel,"maximum",">=","10")
oMyConditions.Logic = "C1"

oMyResultsColumn = oMyDataFinder.CreateResultsColumns()
oMyResultsColumn.RemoveAll()
oMyResultsColumn.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumn.Add(dd.eSearchFile, "fileName")
oMyResultsColumn.Add(dd.eSearchFile, "folder")
oMyResultsColumn.Add(dd.eSearchChannel, "maximum")

oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumn, 200)
oMyResults = oMyDataFinder.ResultsProperties
dd.Navigator.LoadProperty(oMyResults)
oMyResults.Clear()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Clear_ITDMResultsProperties.htm`*

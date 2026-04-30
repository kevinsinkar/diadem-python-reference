---
title: "ITDMResultsProperties.ResultsCount"
description: "Specifies the number of search results for a particular property in a column-oriented search."
---

# ITDMResultsProperties.ResultsCount

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsCount for ResultsProperties

Specifies the number of search results for a particular property in a column-oriented search.

## Signature

```python
obj.ResultsCount
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

oMyResults = oMyDataFinder.ResultsProperties
oMyResults.MaxCount = 200
oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumn)

print("Max number of search results: " + oMyResults.MaxCount + "\r\n" + "Number of search results: " + oMyResults.ResultsCount)

dd.Navigator.LoadProperty(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsCount_ITDMResultsProperties.htm`*

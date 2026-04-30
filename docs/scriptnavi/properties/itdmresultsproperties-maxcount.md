---
title: "ITDMResultsProperties.MaxCount"
description: "Specifies in a column-oriented search the maximum number of search results which DIAdem determines for a specific property."
---

# ITDMResultsProperties.MaxCount

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: MaxCount for ResultsProperties

Specifies in a column-oriented search the maximum number of search results which DIAdem determines for a specific property.

## Signature

```python
obj.MaxCount
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

*Source: `ScriptNavi/properties/navigator_property_MaxCount_ITDMResultsProperties.htm`*

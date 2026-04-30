---
title: "ITDMResultsProperties.Count"
description: "Specifies the number of properties in the search results of a column-oriented search."
---

# ITDMResultsProperties.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for ResultsProperties

Specifies the number of properties in the search results of a column-oriented search.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add(dd.eSearchChannel,"maximum",">=","10")
oMyConditions.Logic = "C1"

oMyResultsColumn = oMyDataFinder.CreateResultsColumns()
oMyResultsColumn.RemoveAll()
oMyResultsColumn.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumn.Add(dd.eSearchFile, "fileName")
oMyResultsColumn.Add(dd.eSearchFile, "folder")
oMyResultsColumn.Add(dd.eSearchChannel, "maximum")

oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumn)
oMyResults = oMyDataFinder.ResultsProperties
dd.MsgBoxDisp("Maximum number of result properties to display: " + oMyResults.MaxCount + "\r\n" + "Number of result properties: " + oMyResults.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMResultsProperties.htm`*

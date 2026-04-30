---
title: "ITDMResultsProperties.IsIncomplete"
description: "Specifies whether the search results list of a column-oriented search contains all properties. If the IsIncomplete property has the value TRUE , the search has "
---

# ITDMResultsProperties.IsIncomplete

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: IsIncomplete for ResultsProperties

Specifies whether the search results list of a column-oriented search contains all properties. If the IsIncomplete property has the value TRUE , the search has more results than the MaxCount property specifies. You only can use the IsIncomplete property if the ResultsProperties object contains search results.

## Signature

```python
obj.IsIncomplete
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

oMyResultsColumns = oMyDataFinder.CreateResultsColumns()
oMyResultsColumns.RemoveAll()
oMyResultsColumns.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumns.Add(dd.eSearchFile, "fileName")
oMyResultsColumns.Add(dd.eSearchFile, "folder")
oMyResultsColumns.Add(dd.eSearchChannel, "maximum")

oMyDataFinder.SearchProperties(oMyQuery, oMyResultsColumns)
oMyResultsProps = oMyDataFinder.ResultsProperties
dd.MsgBoxDisp("Results properties incomplete? " + oMyResultsProps.IsIncomplete)

dd.Navigator.LoadProperty(oMyResultsProps)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_IsIncomplete_ITDMResultsProperties.htm`*

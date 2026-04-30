---
title: "ITDMResultsProperty.Property"
description: "Specifies in a column-oriented search the name of a property in a column of the search results."
---

# ITDMResultsProperty.Property

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Property for ResultsProperty

Specifies in a column-oriented search the name of a property in a column of the search results.

## Signature

```python
obj.Property
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
oMyResult = oMyResults(1)
dd.MsgBoxDisp("Type of Search Result: " + oMyResult.Type + "\r\n" + "Property: " + oMyResult.Property + "\r\n" + "Data Type: " + oMyResult.DataType)
dd.Navigator.LoadProperty(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Property_ITDMResultsProperty.htm`*

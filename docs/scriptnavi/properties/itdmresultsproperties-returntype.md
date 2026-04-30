---
title: "ITDMResultsProperties.ReturnType"
description: "Specifies in a column-oriented search the return type of the property values in the search result."
---

# ITDMResultsProperties.ReturnType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ReturnType for ResultsProperties

Specifies in a column-oriented search the return type of the property values in the search result.

## Signature

```python
obj.ReturnType
```

## Python example

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
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
dd.MsgBoxDisp("Result properties return type: " + oMyResultsProps.ReturnType)

dd.Navigator.LoadProperty(oMyResultsProps)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ReturnType_ITDMResultsProperties.htm`*

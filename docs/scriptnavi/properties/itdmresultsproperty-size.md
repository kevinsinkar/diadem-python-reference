---
title: "ITDMResultsProperty.Size"
description: "Specifies how often a property occurs in the search result of a column-oriented search."
---

# ITDMResultsProperty.Size

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Size for ResultsProperty

Specifies how often a property occurs in the search result of a column-oriented search.

## Signature

```python
obj.Size
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
oMyResultsProp = oMyResultsProps("maximum")
dd.MsgBoxDisp("Size of maximum result property: " + oMyResultsProp.Size)

dd.Navigator.LoadProperty("maximum", oMyResultsProps)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Size_ITDMResultsProperty.htm`*

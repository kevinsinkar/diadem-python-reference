---
title: "ITDMResultsProperty.GetPath"
description: "Returns the path in a column-oriented search with which you can access a property in the search results list. The ReturnType property returns the start point of"
---

# ITDMResultsProperty.GetPath

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetPath for ResultsProperty

Returns the path in a column-oriented search with which you can access a property in the search results list. The ReturnType property returns the start point of the path.

## Signature

```python
sGetPath = Object.GetPath()
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
oMyResultsProp = oMyResultsProps(1)

dd.MsgBoxDisp("Path: " + oMyResultsProp.GetPath)

dd.Navigator.LoadProperty(oMyResultsProps)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetPath_ITDMResultsProperty.htm`*

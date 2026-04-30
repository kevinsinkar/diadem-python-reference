---
title: "ITDMResultsProperty.GetValuesBlock"
description: "Reads a block of values from the search results and writes these values to an array."
---

# ITDMResultsProperty.GetValuesBlock

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetValuesBlock for ResultsProperty

Reads a block of values from the search results and writes these values to an array.

## Signature

```python
vGetValuesBlock = Object.GetValuesBlock([Index], [Count])
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
oMyResults = oMyDataFinder.ResultsProperties(4)

MyColumnArray = oMyResults.GetValuesBlock(1,20)
print(MyColumnArray(10))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetValuesBlock_ITDMResultsProperty.htm`*

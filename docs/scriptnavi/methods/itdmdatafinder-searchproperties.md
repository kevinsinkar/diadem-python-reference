---
title: "ITDMDataFinder.SearchProperties"
description: "Executes in a DataFinder a column-oriented search without the user interface. Use the ResultsProperties property to access the results of a search."
---

# ITDMDataFinder.SearchProperties

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: SearchProperties for DataFinder

Executes in a DataFinder a column-oriented search without the user interface. Use the ResultsProperties property to access the results of a search.

## Signature

```python
obj.SearchProperties(Query, ResultsColumns, [MaxCount])
```

## Python example

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add(dd.eSearchChannel,"maximum","<=","10")
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
```

```python
def ResultsModeToText(Mode):
    select_variable_0 = Mode
    if (select_variable_0 == dd.eResultsModeElements) :
        ResultsModeToText = "eResultsModeElements"
    elif (select_variable_0 == dd.eResultsModeProperties) :
        ResultsModeToText = "eResultsModeProperties"
    else:
        ResultsModeToText = "Error: unknown"
    return ResultsModeToText

print (ResultsModeToText(dd.Navigator.Display.CurrDataFinder.QueryForm.ResultsMode))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_SearchProperties_ITDMDataFinder.htm`*

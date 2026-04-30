---
title: "ITDMResultsProperty"
description: "The ResultsProperty object provides a column with properties in the search results list of a column-oriented search."
---

# ITDMResultsProperty

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ResultsProperty

The ResultsProperty object provides a column with properties in the search results list of a column-oriented search.

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
oMyResult = oMyResults(4)
dd.Navigator.LoadProperty(oMyResult.GetPath, oMyResults)
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

print(ResultsModeToText(dd.Navigator.Display.CurrDataFinder.QueryForm.ResultsMode))
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmresultsproperty-datatype/">DataType</a> | <a href="../../properties/itdmresultsproperty-property/">Property</a> | <a href="../../properties/itdmresultsproperty-size/">Size</a> | <a href="../../properties/itdmresultsproperty-type/">Type</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmresultsproperty-getpath/">GetPath</a> | <a href="../../methods/itdmresultsproperty-getvaluesblock/">GetValuesBlock</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/resultsproperties/">ResultsProperties</a>.<a href="../../methods/itdmresultsproperties-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMResultsProperty.htm`*

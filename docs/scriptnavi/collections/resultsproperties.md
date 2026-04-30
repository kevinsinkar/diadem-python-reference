---
title: "ResultsProperties"
description: "The ResultsProperties object provides the search result of a column-oriented search."
---

# ResultsProperties

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: ResultsProperties

The ResultsProperties object provides the search result of a column-oriented search.

## Python example

```python
dd.Data.Root.Clear()

oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.CreateQuery(dd.eAdvancedQuery)
oMyQuery.ReturnType = dd.eSearchChannel
oMyConditions = oMyQuery.Conditions
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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmresultsproperties-count/">Count</a> | <a href="../../properties/itdmresultsproperties-isincomplete/">IsIncomplete</a> | <a href="../../properties/itdmresultsproperties-maxcount/">MaxCount</a> | <a href="../../properties/itdmresultsproperties-resultscount/">ResultsCount</a> | <a href="../../properties/itdmresultsproperties-returntype/">ReturnType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmresultsproperties-clear/">Clear</a> | <a href="../../methods/itdmresultsproperties-exists/">Exists</a> | <a href="../../methods/itdmresultsproperties-item/">Item</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmdatafinder/">DataFinder</a>.<a href="../../properties/itdmdatafinder-resultsproperties/">ResultsProperties</a> | <a href="../../objects/itdmdatastore/">DataStore</a>.<a href="../../properties/itdmdatastore-resultsproperties/">ResultsProperties</a> | <a href="../../objects/inavidatafinderresultdisplay/">ResultsList &lt;DataFinder&gt;</a>.<a href="../../properties/inavidatafinderresultdisplay-resultsproperties/">ResultsProperties</a> | <a href="../../objects/inavidatastoreresultdisplay/">ResultsList &lt;DataStore&gt;</a>.<a href="../../properties/inavidatastoreresultdisplay-resultsproperties/">ResultsProperties</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMResultsProperties.htm`*

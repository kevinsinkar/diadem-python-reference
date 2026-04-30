---
title: "INaviDataFinderQueryForm.ResultsMode"
description: "Specifies whether you search for elements or execute a column-oriented search for properties on the DataFinder interface."
---

# INaviDataFinderQueryForm.ResultsMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsMode for QueryForm <DataFinder>

Specifies whether you search for elements or execute a column-oriented search for properties on the DataFinder interface.

## Signature

```python
obj.ResultsMode
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you search for elements (<span class="Monospace">ResultsMode</span> = <span class="Monospace">eResultsModeElements)</span>, DIAdem returns the search results in the property <a href="../../objects/inavidatafinderresultdisplay/">ResultsList</a>.<a href="../inavidatafinderresultdisplay-resultselements/">ResultsElements</a>. If you execute a column oriented search (<span class="Monospace">ResultsMode</span> = <span class="Monospace">eResultsModeProperties</span>), DIAdem returns the search results in the property <a href="../../objects/inavidatafinderresultdisplay/">ResultsList</a>.<a href="../inavidatafinderresultdisplay-resultsproperties/">ResultsProperties</a>.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eResultsModeElements` | 1 | Search for elements |
| `eResultsModeProperties` | 2 | Column-oriented search for properties |

## Python example

```python
oMyDataFinder = dd.Navigator.Display.CurrDataFinder
#Configure Queryform
oMyQueryForm  = oMyDataFinder.QueryForm
oMyQueryForm.Clear()
oMyQueryForm.Mode        = dd.eAdvancedQueryForm
oMyQueryForm.ReturnType  = dd.eSearchChannel
oMyQueryForm.ResultsMode = dd.eResultsModeProperties
oMyConditions = oMyQueryForm.Conditions
#Fill the Query
oMyConditions.Add(dd.eSearchChannel,"name","=","*")
oMyConditions.Logic = "C1"
#Define Result Columns
oMyResultsColumns = oMyDataFinder.ResultsList.Settings.Columns
oMyResultsColumn = oMyResultsColumns(dd.eSearchChannel)
#Fill Results Columns
oMyResultsColumn.RemoveAll()
oMyResultsColumn.Add(dd.eSearchChannelGroup, "name")
oMyResultsColumn.Add(dd.eSearchFile, "fileName")
oMyResultsColumn.Add(dd.eSearchChannel, "maximum")
oMyResultsColumn.Add(dd.eSearchChannel, "minimum")
#Search
oMyDataFinder.ResultsList.Settings.MaxCount = 200
oMyQueryForm.Search()
oMyResults = oMyDataFinder.ResultsList.ResultsProperties
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

*Source: `ScriptNavi/properties/navigator_property_ResultsMode_INaviDataFinderQueryForm.htm`*

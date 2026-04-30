---
title: "INaviDataFinderResultDisplay.ResultsProperties"
description: "Specifies the search result of a column-oriented interface search in a DataFinder."
---

# INaviDataFinderResultDisplay.ResultsProperties

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsProperties for ResultsList <DataFinder>

Specifies the search result of a column-oriented interface search in a DataFinder.

## Signature

```python
return_value = obj.ResultsProperties
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you search for elements (<span class="Monospace">ResultsMode</span> = <span class="Monospace">eResultsModeElements)</span>, DIAdem returns the search results in the property <a href="../../objects/inavidatafinderresultdisplay/">ResultsList</a>.<a href="../inavidatafinderresultdisplay-resultselements/">ResultsElements</a>. If you execute a column oriented search (<span class="Monospace">ResultsMode</span> = <span class="Monospace">eResultsModeProperties</span>), DIAdem returns the search results in the property <a href="../../objects/inavidatafinderresultdisplay/">ResultsList</a>.<a href="./">ResultsProperties</a>.</td></tr></table>
</div>

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
dd.MsgBoxDisp(oMyResults.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsProperties_INaviDataFinderResultDisplay.htm`*

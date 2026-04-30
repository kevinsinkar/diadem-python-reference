---
title: "INaviDataFinderResultDisplay.ResultsElements"
description: "Returns a collection of the currently displayed search results in a DataFinder interface search."
---

# INaviDataFinderResultDisplay.ResultsElements

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsElements for ResultsList <DataFinder>

Returns a collection of the currently displayed search results in a DataFinder interface search.

## Signature

```python
return_value = obj.ResultsElements
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <a href="../isusielements-maxcount/">MaxCount</a> property specifies the maximum number of elements that a search returns to the search results. The <a href="../isusielements-isincomplete/">IsIncomplete</a> property specifies whether the search results contain all the search results elements.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  If you search for elements (<span class="Monospace">ResultsMode</span> = <span class="Monospace">eResultsModeElements)</span>, DIAdem returns the search results in the property <a href="../../objects/inavidatafinderresultdisplay/">ResultsList</a>.<a href="./">ResultsElements</a>. If you execute a column oriented search (<span class="Monospace">ResultsMode</span> = <span class="Monospace">eResultsModeProperties</span>), DIAdem returns the search results in the property <a href="../../objects/inavidatafinderresultdisplay/">ResultsList</a>.<a href="../inavidatafinderresultdisplay-resultsproperties/">ResultsProperties</a>.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.Display.CurrDataFinder
oMyQuery = oMyDataFinder.QueryForm
oMyQuery.ReturnType = dd.eSearchChannel
oMyQueryForm = oMyDataFinder.QueryForm
oMyQueryForm.ResultsMode = dd.eResultsModeElements

oMyConditions = oMyQuery.Conditions
oMyConditions.RemoveAll()
oMyConditions.Add(dd.eSearchChannel,"unit_string","=","Hz")
oMyConditions.Logic = "C1"

oMyDataFinder.QueryForm.Search()
oMyResultsList = oMyDataFinder.ResultsList
dd.MsgBoxDisp("Number of results: " + oMyResultsList.ResultsElements.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsElements_INaviDataFinderResultDisplay.htm`*

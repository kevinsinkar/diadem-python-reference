---
title: "ITDMDataFinder.ResultsElements"
description: "Returns in a DataFinder the search results of a search without user interface for elements."
---

# ITDMDataFinder.ResultsElements

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsElements for DataFinder

Returns in a DataFinder the search results of a search without user interface for elements.

## Signature

```python
return_value = obj.ResultsElements
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  The <a href="../isusielements-maxcount/">MaxCount</a> property specifies the maximum number of elements that a search returns to the search results. The <a href="../isusielements-isincomplete/">IsIncomplete</a> property specifies whether the search results contain all the search results elements.</td></tr></table>
</div>

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
dd.Navigator.LoadData(oMyResults)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsElements_ITDMDataFinder.htm`*

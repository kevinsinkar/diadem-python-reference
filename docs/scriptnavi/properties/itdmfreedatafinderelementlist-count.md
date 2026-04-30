---
title: "ITDMFreeDataFinderElementList.Count"
description: "Returns in the DIAdem NAVIGATOR script interface the number of elements of a FreeElementList collection."
---

# ITDMFreeDataFinderElementList.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for FreeElementList <DataFinder>

Returns in the DIAdem NAVIGATOR script interface the number of elements of a FreeElementList collection.

## Signature

```python
obj.Count
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList = oMyDataFinder.CreateElementList()
oMyElementList.AddElementList(oMyResults)
dd.MsgBoxDisp(oMyElementList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMFreeDataFinderElementList.htm`*

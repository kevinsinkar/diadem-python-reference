---
title: "ITDMFreeDataFinderElementList.RemoveAll"
description: "Deletes in the object-oriented script interface of DIAdem NAVIGATOR all elements from the ElementList collection of a DataFinder. This method is not available i"
---

# ITDMFreeDataFinderElementList.RemoveAll

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: RemoveAll for FreeElementList <DataFinder>

Deletes in the object-oriented script interface of DIAdem NAVIGATOR all elements from the ElementList collection of a DataFinder. This method is not available if the ElementList collection is read-only.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList = oMyDataFinder.CreateElementList()
oMyElementList.AddElementList(oMyResults)
oMyElementList.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_RemoveAll_ITDMFreeDataFinderElementList.htm`*

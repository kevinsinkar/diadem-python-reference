---
title: "ITDMFreeDataFinderElementList.Remove"
description: "Deletes in the object-oriented script interface of DIAdem NAVIGATOR an element from the ElementList collection of a DataFinder. This method is not available if "
---

# ITDMFreeDataFinderElementList.Remove

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Remove for FreeElementList <DataFinder>

Deletes in the object-oriented script interface of DIAdem NAVIGATOR an element from the ElementList collection of a DataFinder. This method is not available if the ElementList collection is read-only.

## Signature

```python
obj.Remove(ElementOrIndex)
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList = oMyDataFinder.CreateElementList()
oMyElementList.AddElementList(oMyResults)
oMyElementList.Remove(1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Remove_ITDMFreeDataFinderElementList.htm`*

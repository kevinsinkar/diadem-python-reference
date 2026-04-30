---
title: "ITDMFreeDataFinderElementList.Item"
description: "Returns in the object-oriented script interface of DIAdem NAVIGATOR a data store's FreeElementList object associated with a specific index."
---

# ITDMFreeDataFinderElementList.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for FreeElementList <DataFinder>

Returns in the object-oriented script interface of DIAdem NAVIGATOR a data store's FreeElementList object associated with a specific index.

## Signature

```python
return_value = obj.Item(Index)
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList = oMyDataFinder.CreateElementList()
oMyElementList.AddElementList(oMyResults)
dd.MsgBoxDisp(oMyElementList.Item(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_ITDMFreeDataFinderElementList.htm`*

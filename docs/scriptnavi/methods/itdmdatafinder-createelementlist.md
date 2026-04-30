---
title: "ITDMDataFinder.CreateElementList"
description: "Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of DataFinder elements. Each element in the created collection is an Element <D"
---

# ITDMDataFinder.CreateElementList

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateElementList for DataFinder

Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of DataFinder elements. Each element in the created collection is an Element <DataFinder> > .

## Signature

```python
return_value = obj.CreateElementList()
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

*Source: `ScriptNavi/methods/navigator_method_CreateElementList_ITDMDataFinder.htm`*

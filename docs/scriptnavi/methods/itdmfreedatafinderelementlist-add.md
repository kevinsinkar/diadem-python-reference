---
title: "ITDMFreeDataFinderElementList.Add"
description: "Adds in the object-oriented script interface of DIAdem NAVIGATOR a new element to the FreeElementList collection of a DataFinder. The Add method returns a <Data"
---

# ITDMFreeDataFinderElementList.Add

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Add for FreeElementList <DataFinder>

Adds in the object-oriented script interface of DIAdem NAVIGATOR a new element to the FreeElementList collection of a DataFinder. The Add method returns a <DataFinder>object. This method is not available if the FreeElementList collection is read-only.

## Signature

```python
return_value = obj.Add(Element)
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyElementList = oMyDataFinder.CreateElementList()
oMyResults = oMyDataFinder.ResultsElements
for oMyResult in oMyResults:
    oMyElementList.Add(oMyResult)
dd.MsgBoxDisp(oMyElementList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Add_ITDMFreeDataFinderElementList.htm`*

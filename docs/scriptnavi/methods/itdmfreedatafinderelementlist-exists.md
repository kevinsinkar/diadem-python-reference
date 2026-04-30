---
title: "ITDMFreeDataFinderElementList.Exists"
description: "Checks in the object-oriented script-interface of DIAdem NAVIGATOR in the DataFinder elements list whether a certain element already exists in the list."
---

# ITDMFreeDataFinderElementList.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for FreeElementList <DataFinder>

Checks in the object-oriented script-interface of DIAdem NAVIGATOR in the DataFinder elements list whether a certain element already exists in the list.

## Signature

```python
bExists = Object.Exists(Element)
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")
oMyElementList1 = oMyDataFinder.CreateElementList()
oMyElementList2 = oMyDataFinder.CreateElementList()
oMyQuery = oMyDataFinder.LoadQuery(dd.ConfReadPath + "Query_Example.tdq")
oMyDataFinder.SearchElements(oMyQuery)
oMyResults = oMyDataFinder.ResultsElements
for oMyResult in oMyResults:
    if not oMyElementList1.Exists(oMyResult) :
        oMyElementList1.Add(oMyResult)
for oMyResult in oMyResults:
    oMyElementList2.Add(oMyResult)
oMyElementList1.AddElementList(oMyElementList2,dd.ListMergeModeAdd)
dd.MsgBoxDisp("Sum of Elements: " + oMyElementList1.Count )
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ITDMFreeDataFinderElementList.htm`*

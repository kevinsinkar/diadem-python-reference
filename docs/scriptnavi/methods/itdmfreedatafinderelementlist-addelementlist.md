---
title: "ITDMFreeDataFinderElementList.AddElementList"
description: "Connects in the object-oriented script interface in DIAdem NAVIGATOR two element lists of a DataFinder."
---

# ITDMFreeDataFinderElementList.AddElementList

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: AddElementList for FreeElementList <DataFinder>

Connects in the object-oriented script interface in DIAdem NAVIGATOR two element lists of a DataFinder.

## Signature

```python
obj.AddElementList(DataFinderElementList, [ListMergeMode])
```

## Python example

```python
oMyDataFinder = dd.Navigator.ConnectDataFinder("My DataFinder")

#First Query
oMyQuery1 = oMyDataFinder.CreateQuery(dd.eTextQuery)
oMyQuery1.Text = "TR_M17_QT_32-1"
oMyDataFinder.SearchElements(oMyQuery1)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList1 = oMyDataFinder.CreateElementList()
oMyElementList1.AddElementList(oMyResults)

#Second Query
oMyQuery2 = oMyDataFinder.CreateQuery(dd.eTextQuery)
oMyQuery2.Text = "TR_M17_QT_32-4"
oMyDataFinder.SearchElements(oMyQuery2)
oMyResults = oMyDataFinder.ResultsElements
oMyElementList2 = oMyDataFinder.CreateElementList()
oMyElementList2.AddElementList(oMyResults)

#Combining via ListMergeModeAdd
oMyElementList1.AddElementList(oMyElementList2, dd.ListMergeModeAdd)
dd.MsgBoxDisp("Sum of Elements (ListMergeModeAdd): " + oMyElementList1.Count)

#Combining via ListMergeModeIntersection
oMyElementList1.AddElementList(oMyElementList2, dd.ListMergeModeIntersection)
dd.MsgBoxDisp("Sum of Elements (ListMergeModeIntersection): " + oMyElementList1.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_AddElementList_ITDMFreeDataFinderElementList.htm`*

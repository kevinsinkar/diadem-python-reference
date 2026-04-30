---
title: "ITDMFreeStoreElementList.AddElementList"
description: "Connects in the object-oriented script interface in DIAdem NAVIGATOR two element lists of a data store."
---

# ITDMFreeStoreElementList.AddElementList

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: AddElementList for FreeElementList <DataStore>

Connects in the object-oriented script interface in DIAdem NAVIGATOR two element lists of a data store.

## Signature

```python
obj.AddElementList(StoreElementList, [ListMergeMode])
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)

#First Query
oMyQuery1 = oMyDataStore.CreateQuery(dd.eDataStoreQuery)
oMyQuery1.Conditions.Add("measurement","name","=","QT_32-1_Lower")
oMyDataStore.SearchElements(oMyQuery1)
oMyResults = oMyDataStore.ResultsElements
oMyElementList1 = oMyDataStore.CreateElementList()
oMyElementList1.AddElementList(oMyResults)

#Second Query
oMyQuery2 = oMyDataStore.CreateQuery(dd.eDataStoreQuery)
oMyQuery2.Conditions.Add("measurement","name","=","QT_34-9_Upper")
oMyDataStore.SearchElements(oMyQuery2)
oMyResults = oMyDataStore.ResultsElements
oMyElementList2 = oMyDataStore.CreateElementList()
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

*Source: `ScriptNavi/methods/navigator_method_AddElementList_ITDMFreeStoreElementList.htm`*

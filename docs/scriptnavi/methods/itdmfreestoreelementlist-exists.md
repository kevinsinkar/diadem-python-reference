---
title: "ITDMFreeStoreElementList.Exists"
description: "Checks in the object-oriented script-interface of DIAdem NAVIGATOR in a data store's elements list whether a certain element already exists in the list."
---

# ITDMFreeStoreElementList.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for FreeElementList <DataStore>

Checks in the object-oriented script-interface of DIAdem NAVIGATOR in a data store's elements list whether a certain element already exists in the list.

## Signature

```python
bExists = Object.Exists(Element)
```

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyElementList1 = oMyStore.CreateElementList()
oMyElementList2 = oMyStore.CreateElementList()
oMyQuery = oMyStore.LoadQuery(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq")
oMyStore.SearchElements(oMyQuery)
oMyResults = oMyStore.ResultsElements
for oMyResult in oMyResults:
    if not oMyElementList1.Exists(oMyResult) :
        oMyElementList1.Add(oMyResult)
for oMyResult in oMyResults:
    oMyElementList2.Add(oMyResult)
oMyElementList1.AddElementList(oMyElementList2,dd.ListMergeModeAdd)
dd.MsgBoxDisp("Sum of Elements: " + oMyElementList1.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ITDMFreeStoreElementList.htm`*

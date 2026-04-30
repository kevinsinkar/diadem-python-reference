---
title: "ITDMFreeStoreElementList.Add"
description: "Adds in the object-oriented script interface of DIAdem NAVIGATOR a new element to the FreeElementList collection of a data store. The Add method returns an Elem"
---

# ITDMFreeStoreElementList.Add

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Add for FreeElementList <DataStore>

Adds in the object-oriented script interface of DIAdem NAVIGATOR a new element to the FreeElementList collection of a data store. The Add method returns an Element <DataStore> object. This method is not available if the FreeElementList collection is read-only.

## Signature

```python
return_value = obj.Add(Element)
```

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyQuery = oMyStore.LoadQuery(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq")
oMyStore.SearchElements(oMyQuery)
oMyElementList = oMyStore.CreateElementList()
oMyResults = oMyStore.ResultsElements
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

*Source: `ScriptNavi/methods/navigator_method_Add_ITDMFreeStoreElementList.htm`*

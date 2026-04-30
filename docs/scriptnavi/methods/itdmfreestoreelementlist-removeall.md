---
title: "ITDMFreeStoreElementList.RemoveAll"
description: "Deletes in the object-oriented script interface of DIAdem NAVIGATOR all elements from the ElementList collection of a data store. This method is not available i"
---

# ITDMFreeStoreElementList.RemoveAll

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: RemoveAll for FreeElementList <DataStore>

Deletes in the object-oriented script interface of DIAdem NAVIGATOR all elements from the ElementList collection of a data store. This method is not available if the ElementList collection is read-only.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyQuery = oMyStore.LoadQuery(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq")
oMyStore.SearchElements(oMyQuery)
oMyResults = oMyStore.ResultsElements
oMyElementList = oMyStore.CreateElementList()
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

*Source: `ScriptNavi/methods/navigator_method_RemoveAll_ITDMFreeStoreElementList.htm`*

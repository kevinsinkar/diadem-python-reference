---
title: "ITDMFreeStoreElementList.Count"
description: "Returns in the DIAdem NAVIGATOR script interface the number of elements of a data store's FreeElementList collection."
---

# ITDMFreeStoreElementList.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for FreeElementList <DataStore>

Returns in the DIAdem NAVIGATOR script interface the number of elements of a data store's FreeElementList collection.

## Signature

```python
obj.Count
```

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyElementList = oMyStore.CreateElementList()
oMyQuery = oMyStore.LoadQuery(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq")
oMyStore.SearchElements(oMyQuery)
oMyResults = oMyStore.ResultsElements
oMyElementList.AddElementlist(oMyResults)
dd.MsgBoxDisp(oMyElementList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMFreeStoreElementList.htm`*

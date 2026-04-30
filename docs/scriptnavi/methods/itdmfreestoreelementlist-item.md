---
title: "ITDMFreeStoreElementList.Item"
description: "Returns in the object-oriented script interface of DIAdem NAVIGATOR the DataFinder's FreeElementList object of a specific index."
---

# ITDMFreeStoreElementList.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for FreeElementList <DataStore>

Returns in the object-oriented script interface of DIAdem NAVIGATOR the DataFinder's FreeElementList object of a specific index.

## Signature

```python
return_value = obj.Item(Index)
```

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyQuery = oMyStore.LoadQuery(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq")
oMyStore.SearchElements(oMyQuery)
oMyResults = oMyStore.ResultsElements
oMyElementList = oMyStore.CreateElementList()
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

*Source: `ScriptNavi/methods/navigator_method_Item_ITDMFreeStoreElementList.htm`*

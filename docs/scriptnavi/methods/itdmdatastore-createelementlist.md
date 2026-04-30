---
title: "ITDMDataStore.CreateElementList"
description: "Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of data store elements. Each element in the created collection is an Element <D"
---

# ITDMDataStore.CreateElementList

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: CreateElementList for DataStore

Creates in the object-oriented script interface of DIAdem NAVIGATOR a collection of data store elements. Each element in the created collection is an Element <DataStore> .

## Signature

```python
return_value = obj.CreateElementList()
```

## Python example

```python
oMyStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example " + dd.ProgramVersionName)
oMyQuery = oMyStore.LoadQuery(dd.CommonDocumentsPath + "Documents\\Query_Example_ASAM.tdq")
oMyStore.SearchElements(oMyQuery)
oMyResults = oMyStore.ResultsElements
oMyElementList = oMyStore.CreateElementList()
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

*Source: `ScriptNavi/methods/navigator_method_CreateElementList_ITDMDataStore.htm`*

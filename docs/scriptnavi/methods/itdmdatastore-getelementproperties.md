---
title: "ITDMDataStore.GetElementProperties"
description: "Returns a list with all properties which fulfill a specific search condition in a data store."
---

# ITDMDataStore.GetElementProperties

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetElementProperties for DataStore

Returns a list with all properties which fulfill a specific search condition in a data store.

## Signature

```python
obj.GetElementProperties(ReturnType, QueryExpression, ResultsColumns, [MaxCount])
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")

oMyResultsColumn = oMyDataStore.CreateResultsColumns()
oMyResultsColumn.RemoveAll()
oMyResultsColumn.Add("Measurement", "name")
oMyResultsColumn.Add("MeaQuantity", "Id")

oMyDataStore.GetElementProperties("MeaQuantity", "Name=Time", oMyResultsColumn, 200)
for MyProperty in oMyDataStore.ResultsProperties:
    dd.MsgBoxDisp(MyProperty.GetPath)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetElementProperties_ITDMDataStore.htm`*

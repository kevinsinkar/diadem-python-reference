---
title: "IDataStoreTextQuery.ReturnType"
description: "Specifies the search results type of a search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is decl"
---

# IDataStoreTextQuery.ReturnType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ReturnType for TextQuery <DataStore>

Specifies the search results type of a search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server. The search results of a quick search in a data store is always a test type.

## Signature

```python
obj.ReturnType
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("AsamTest1")
oMyQuery = oMyDataStore.CreateQuery(dd.eDataStoreTextQuery)
oMyQuery.Text = "SearchValue"
dd.MsgBoxDisp(oMyQuery.ReturnType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ReturnType_IDataStoreTextQuery.htm`*

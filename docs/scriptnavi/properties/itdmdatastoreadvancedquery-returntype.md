---
title: "ITDMDataStoreAdvancedQuery.ReturnType"
description: "Specifies the search results type in an advanced search in a data store."
---

# ITDMDataStoreAdvancedQuery.ReturnType

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ReturnType for AdvancedQuery <DataStore>

Specifies the search results type in an advanced search in a data store.

## Signature

```python
obj.ReturnType
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Pass Fail Analysis Example "+ dd.ProgramVersionName)
oMyQuery = oMyDataStore.CreateQuery(dd.eDataStoreQuery)
oMyQuery.Conditions.Add("MeaQuantity","name","=","data*")
dd.LogfileWrite(oMyQuery.ReturnType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ReturnType_ITDMDataStoreAdvancedQuery.htm`*

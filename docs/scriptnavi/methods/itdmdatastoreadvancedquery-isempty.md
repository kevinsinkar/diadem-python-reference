---
title: "ITDMDataStoreAdvancedQuery.IsEmpty"
description: "Determines in an advanced search in a data store whether the search conditions of a search object are empty."
---

# ITDMDataStoreAdvancedQuery.IsEmpty

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsEmpty for AdvancedQuery <DataStore>

Determines in an advanced search in a data store whether the search conditions of a search object are empty.

## Signature

```python
bIsEmpty = Object.IsEmpty()
```

## Python example

```python
oMyDataStore= dd.Navigator.Display.CurrDataStore
oMyQuery = oMyDataStore.QueryForm.GetCurrQuery()
if (not oMyQuery.IsEmpty) :
    oMyDataStore.SaveQueryInfoSet(dd.ConfWritePath + "MyQuery.tdq")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsEmpty_ITDMDataStoreAdvancedQuery.htm`*

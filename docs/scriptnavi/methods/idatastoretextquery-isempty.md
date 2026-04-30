---
title: "IDataStoreTextQuery.IsEmpty"
description: "Determines when running a quick search in a data store whether the search text of a search object is empty. You can execute a quick search only on a DataFinder "
---

# IDataStoreTextQuery.IsEmpty

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsEmpty for TextQuery <DataStore>

Determines when running a quick search in a data store whether the search text of a search object is empty. You can execute a quick search only on a DataFinder instance which is declared as an ASAM ODS server.

## Signature

```python
bIsEmpty = Object.IsEmpty
```

## Python example

```python
oMyDataStore = dd.Navigator.Display.CurrDataStore
oMyQuery = oMyDataStore.QueryForm.GetCurrQuery()
if (not oMyQuery.IsEmpty) :
    oMyDataStore.SaveQueryInfoSet("D:\\MyQuery.tdq")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsEmpty_IDataStoreTextQuery.htm`*

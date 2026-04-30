---
title: "IDataStoreTextQuery.Text"
description: "Specifies the search text for the quick search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is dec"
---

# IDataStoreTextQuery.Text

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Text for TextQuery <DataStore>

Specifies the search text for the quick search in a data store. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server.

## Signature

```python
obj.Text
```

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("AsamTest1")
oMyQuery = oMyDataStore.CreateQuery(dd.eDataStoreTextQuery)
oMyQuery.Text = "SearchValue"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Text_IDataStoreTextQuery.htm`*

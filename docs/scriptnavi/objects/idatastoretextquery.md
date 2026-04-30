---
title: "IDataStoreTextQuery"
description: "The TextQuery object provides the properties for a quick search in a data store. If you execute a quick search, DIAdem searches to the specified value in all pr"
---

# IDataStoreTextQuery

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: TextQuery <DataStore>

The TextQuery object provides the properties for a quick search in a data store. If you execute a quick search, DIAdem searches to the specified value in all properties. You can only run a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server.

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("AsamTest1")
oMyTextQuery = oMyDataStore.CreateQuery(dd.eDataStoreTextQuery)
oMyTextQuery.Text = "SearchValue"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/idatastoretextquery-returntype/">ReturnType</a> | <a href="../../properties/idatastoretextquery-text/">Text</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/idatastoretextquery-isempty/">IsEmpty</a> | <a href="../../methods/idatastoretextquery-iskindof/">IsKindOf</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_IDataStoreTextQuery.htm`*

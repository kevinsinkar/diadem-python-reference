---
title: "INaviDataStoreQueryForm.Mode"
description: "Specifies whether DIAdem displays in a data store the quick search or the advanced search for properties. By default DIAdem uses the advanced search to search f"
---

# INaviDataStoreQueryForm.Mode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Mode for QueryForm <DataStore>

Specifies whether DIAdem displays in a data store the quick search or the advanced search for properties. By default DIAdem uses the advanced search to search for elements. You can only execute a quick search in a data store if you access a DataFinder instance which is declared as an ASAM ODS server.

## Signature

```python
obj.Mode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAdvancedQueryForm` | 1 | Advanced search for elements |
| `eQuickQueryForm` | 2 | Quick search |

## Python example

```python
dd.Navigator.Display.CurrDataStore.QueryForm.Mode = dd.eQuickQueryForm
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Mode_INaviDataStoreQueryForm.htm`*

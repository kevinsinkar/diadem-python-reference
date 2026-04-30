---
title: "INaviDataStoreQueryForm.ResultsMode"
description: "Specifies whether you search for data elements or execute a column-oriented search for properties on the data store interface. If you search for elements ( Resu"
---

# INaviDataStoreQueryForm.ResultsMode

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: ResultsMode for QueryForm <DataStore>

Specifies whether you search for data elements or execute a column-oriented search for properties on the data store interface. If you search for elements ( ResultsMode = eResultsModeElements) , DIAdem returns the search results in the property ResultsList . ResultsElements . If you execute a column oriented search ( ResultsMode = eResultsModeProperties ), DIAdem returns the search results in the property ResultsList . ResultsProperties .

## Signature

```python
obj.ResultsMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eResultsModeElements` | 1 | Search for data elements |
| `eResultsModeProperties` | 2 | Column-oriented search for properties |

## Python example

```python
oMyDataStore = dd.Navigator.Display.CurrDataStore
oMyQueryForm = oMyDataStore.QueryForm
oMyQueryForm.ResultsMode = dd.eResultsModeElements
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_ResultsMode_INaviDataStoreQueryForm.htm`*

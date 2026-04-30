---
title: "ITDMStoreProperty.GetLowBytes"
description: "Returns the lowest 4 bytes of a data element property that is an Int64 type in a data store in DIAdem NAVIGATOR."
---

# ITDMStoreProperty.GetLowBytes

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetLowBytes for Property <DataStore>

Returns the lowest 4 bytes of a data element property that is an Int64 type in a data store in DIAdem NAVIGATOR.

## Signature

```python
iGetLowBytes = Object.GetLowBytes()
```

## Python example

```python
LowBytes = dd.Navigator.Display.CurrDataStore.Browser.SelectedElements(1).Properties("Id").GetLowBytes()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetLowBytes_ITDMStoreProperty.htm`*

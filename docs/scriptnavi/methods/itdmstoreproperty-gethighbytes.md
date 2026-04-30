---
title: "ITDMStoreProperty.GetHighBytes"
description: "Returns the highest 4 bytes of a data element property that is an Int64 type in a data store in DIAdem NAVIGATOR."
---

# ITDMStoreProperty.GetHighBytes

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: GetHighBytes for Property <DataStore>

Returns the highest 4 bytes of a data element property that is an Int64 type in a data store in DIAdem NAVIGATOR.

## Signature

```python
iGetHighBytes = Object.GetHighBytes()
```

## Python example

```python
LowBytes = dd.Navigator.Display.CurrDataStore.Browser.SelectedElements(1).Properties("Id").GetHighBytes()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_GetHighBytes_ITDMStoreProperty.htm`*

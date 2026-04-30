---
title: "ITDMDataStore.IsValid"
description: "Specifies whether a data store object is currently valid in DIAdem NAVIGATOR."
---

# ITDMDataStore.IsValid

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsValid for DataStore

Specifies whether a data store object is currently valid in DIAdem NAVIGATOR.

## Signature

```python
bIsValid = Object.IsValid()
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
dd.MsgBoxDisp("DataStore " + oMyDataStore.Name + "is valid: " + oMyDataStore.IsValid)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsValid_ITDMDataStore.htm`*

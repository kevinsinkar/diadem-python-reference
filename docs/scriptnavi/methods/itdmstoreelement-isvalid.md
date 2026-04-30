---
title: "ITDMStoreElement.IsValid"
description: "Specifies whether the element object of a data store is valid."
---

# ITDMStoreElement.IsValid

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsValid for Element <DataStore>

Specifies whether the element object of a data store is valid.

## Signature

```python
bIsValid = Object.IsValid()
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyRootElement = oMyDataStore.RootElements(1)
dd.MsgBoxDisp(oMyRootElement.IsValid)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsValid_ITDMStoreElement.htm`*

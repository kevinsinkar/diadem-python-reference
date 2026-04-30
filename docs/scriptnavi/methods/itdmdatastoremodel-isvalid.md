---
title: "ITDMDataStoreModel.IsValid"
description: "Specifies whether the object which contains the data model of a data store is valid."
---

# ITDMDataStoreModel.IsValid

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsValid for DataStoreModel

Specifies whether the object which contains the data model of a data store is valid.

## Signature

```python
bIsValid = Object.IsValid()
```

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
dd.MsgBoxDisp(oMyDataStoreModel.IsValid)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsValid_ITDMDataStoreModel.htm`*

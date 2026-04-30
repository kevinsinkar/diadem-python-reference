---
title: "ITDMModelEntity.IsValid"
description: "Specifies whether an entity object of a data model is valid."
---

# ITDMModelEntity.IsValid

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsValid for ModelEntity

Specifies whether an entity object of a data model is valid.

## Signature

```python
bIsValid = Object.IsValid()
```

## Python example

```python
oMyDataStore = dd.NAVIGATOR.ConnectDataStore("ASAM Browse Settings Example")
oMyModel = oMyDataStore.Model
oMyEntity = oMyModel.Entities(1)
dd.MsgBoxDisp("Entity valid: " + oMyEntity.IsValid)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsValid_ITDMModelEntity.htm`*

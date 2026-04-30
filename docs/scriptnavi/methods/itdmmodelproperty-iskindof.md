---
title: "ITDMModelProperty.IsKindOf"
description: "Determines whether a property of a ModelEntity in a data store is the specified type."
---

# ITDMModelProperty.IsKindOf

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: IsKindOf for ModelProperty

Determines whether a property of a ModelEntity in a data store is the specified type.

## Signature

```python
bIsKindOf = Object.IsKindOf(PropertyType)
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyDataStoreModel = oMyDataStore.Model
oMyFirstModelEntityProperties = oMyDataStoreModel.Entities("MeaQuantity").ModelProperties
for oProperty in oMyFirstModelEntityProperties:
    if oProperty.IsKindOf("ModelEnumerationProperty") :
        print("Enumeration Property: " + oProperty.Name)
    elif oProperty.IsKindOf("ModelStandardProperty") :
        print("Standard Property: " + oProperty.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_IsKindOf_ITDMModelProperty.htm`*

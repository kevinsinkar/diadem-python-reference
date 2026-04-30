---
title: "ITDMDataStoreModel.Enumerations"
description: "Specifies the enumerations in the model of a data store."
---

# ITDMDataStoreModel.Enumerations

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Enumerations for DataStoreModel

Specifies the enumerations in the model of a data store.

## Signature

```python
return_value = obj.Enumerations
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnums = oMyDataStore.Model.Enumerations
print(oMyEnums.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Enumerations_ITDMDataStoreModel.htm`*

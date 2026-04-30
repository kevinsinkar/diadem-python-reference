---
title: "ITDMModelEnumerationProperty.Enumeration"
description: "Returns an enumeration property in the data model of a data store."
---

# ITDMModelEnumerationProperty.Enumeration

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Enumeration for ModelEnumerationProperty

Returns an enumeration property in the data model of a data store.

## Signature

```python
return_value = obj.Enumeration
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

*Source: `ScriptNavi/properties/navigator_property_Enumeration_ITDMModelEnumerationProperty.htm`*

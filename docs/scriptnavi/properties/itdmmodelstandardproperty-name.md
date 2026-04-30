---
title: "ITDMModelStandardProperty.Name"
description: "Specifies the name of a standard property in an entity of the data model."
---

# ITDMModelStandardProperty.Name

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Name for ModelStandardProperty

Specifies the name of a standard property in an entity of the data model.

## Signature

```python
obj.Name
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

*Source: `ScriptNavi/properties/navigator_property_Name_ITDMModelStandardProperty.htm`*

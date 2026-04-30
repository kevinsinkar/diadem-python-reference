---
title: "ITDMModelEnumeration.Name"
description: "Returns the name of an element of an enumeration in the model of a data store."
---

# ITDMModelEnumeration.Name

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Name for ModelEnumeration

Returns the name of an element of an enumeration in the model of a data store.

## Signature

```python
obj.Name
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
print(oMyDataStore.Model.Enumerations.Item(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Name_ITDMModelEnumeration.htm`*

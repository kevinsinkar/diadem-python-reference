---
title: "ITDMModelEnumeration.Items"
description: "Returns an element of a enumeration in the model of a data store."
---

# ITDMModelEnumeration.Items

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Items for ModelEnumeration

Returns an element of a enumeration in the model of a data store.

## Signature

```python
return_value = obj.Items
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnumItems = oMyDataStore.Model.Enumerations.Item(1).Items
print(oMyEnumItems.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Items_ITDMModelEnumeration.htm`*

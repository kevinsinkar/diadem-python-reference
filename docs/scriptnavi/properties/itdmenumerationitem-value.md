---
title: "ITDMEnumerationItem.Value"
description: "Specifies the value of an element in an enumeration in the model of a data store."
---

# ITDMEnumerationItem.Value

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Value for EnumerationItem

Specifies the value of an element in an enumeration in the model of a data store.

## Signature

```python
obj.Value
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnumItem = oMyDataStore.Model.Enumerations.Item(1).Items(1)
print("Definition: " + oMyEnumItem.Definition + "\r\n" + "Value: " + oMyEnumItem.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/properties/navigator_property_Value_ITDMEnumerationItem.htm`*

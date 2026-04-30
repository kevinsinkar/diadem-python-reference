---
title: "ITDMEnumerationItem.Definition"
description: "Specifies the definition of an element in an enumeration in the model of a data store."
---

# ITDMEnumerationItem.Definition

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Definition for EnumerationItem

Specifies the definition of an element in an enumeration in the model of a data store.

## Signature

```python
obj.Definition
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

*Source: `ScriptNavi/properties/navigator_property_Definition_ITDMEnumerationItem.htm`*

---
title: "ITDMEnumerationItems.Count"
description: "Specifies the number of elements in an enumeration in the model of a data store."
---

# ITDMEnumerationItems.Count

!!! abstract "Property &middot; `ScriptNavi.chm`"
    Property: Count for EnumerationItems

Specifies the number of elements in an enumeration in the model of a data store.

## Signature

```python
obj.Count
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

*Source: `ScriptNavi/properties/navigator_property_Count_ITDMEnumerationItems.htm`*

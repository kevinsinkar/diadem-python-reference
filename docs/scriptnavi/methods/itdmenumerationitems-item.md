---
title: "ITDMEnumerationItems.Item"
description: "Returns in the model of a data store an enumeration element belonging to a specific index or to a specific definition."
---

# ITDMEnumerationItems.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for EnumerationItems

Returns in the model of a data store an enumeration element belonging to a specific index or to a specific definition.

## Signature

```python
return_value = obj.Item(IndexOrDefinition)
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

*Source: `ScriptNavi/methods/navigator_method_Item_ITDMEnumerationItems.htm`*

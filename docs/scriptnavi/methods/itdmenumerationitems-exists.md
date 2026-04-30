---
title: "ITDMEnumerationItems.Exists"
description: "Checks whether a specific element in an enumeration property of the model of a data store already exists."
---

# ITDMEnumerationItems.Exists

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Exists for EnumerationItems

Checks whether a specific element in an enumeration property of the model of a data store already exists.

## Signature

```python
bExists = Object.Exists(Definition)
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnumItems = oMyDataStore.Model.Enumerations("datatype").Items
print(oMyEnumItems.Exists("DT_String"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Exists_ITDMEnumerationItems.htm`*

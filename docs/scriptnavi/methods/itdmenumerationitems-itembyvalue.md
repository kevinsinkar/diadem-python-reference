---
title: "ITDMEnumerationItems.ItemByValue"
description: "Returns an element of an enumeration according to the associated value."
---

# ITDMEnumerationItems.ItemByValue

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: ItemByValue for EnumerationItems

Returns an element of an enumeration according to the associated value.

## Signature

```python
return_value = obj.ItemByValue(Value)
```

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnumItems = oMyDataStore.Model.Enumerations("datatype").Items
print(oMyEnumItems.ItemByValue(2).Definition , "\r\n" , oMyEnumItems.ItemByValue(2).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_ItemByValue_ITDMEnumerationItems.htm`*

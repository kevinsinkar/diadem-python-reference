---
title: "ITDMModelEnumeration"
description: "The ModelEnumeration object provides an enumeration in the model of a data store."
---

# ITDMModelEnumeration

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: ModelEnumeration

The ModelEnumeration object provides an enumeration in the model of a data store.

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnum = oMyDataStore.Model.Enumerations.Item(1)
print(oMyEnum.Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmmodelenumeration-items/">Items</a> | <a href="../../properties/itdmmodelenumeration-name/">Name</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itdmmodelenumerationproperty/">ModelEnumerationProperty</a>.<a href="../../properties/itdmmodelenumerationproperty-enumeration/">Enumeration</a> | <a href="../../collections/modelenumerations/">ModelEnumerations</a>.<a href="../../methods/itdmmodelenumerations-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMModelEnumeration.htm`*

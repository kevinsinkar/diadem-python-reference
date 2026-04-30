---
title: "ITDMEnumerationItem"
description: "The EnumerationItem object provides an element of an enumeration in the model of a data store."
---

# ITDMEnumerationItem

!!! abstract "Object &middot; `ScriptNavi.chm`"
    Object: EnumerationItem

The EnumerationItem object provides an element of an enumeration in the model of a data store.

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnumItem = oMyDataStore.Model.Enumerations.Item(1).Items(1)
print("Definition: " + oMyEnumItem.Definition + "\r\n" + "Value: " + oMyEnumItem.Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmenumerationitem-definition/">Definition</a> | <a href="../../properties/itdmenumerationitem-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/enumerationitems/">EnumerationItems</a>.<a href="../../methods/itdmenumerationitems-item/">Item</a> | <a href="../../collections/enumerationitems/">EnumerationItems</a>.<a href="../../methods/itdmenumerationitems-itembyvalue/">ItemByValue</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMEnumerationItem.htm`*

---
title: "EnumerationItems"
description: "Elements of a enumeration in the model of a data store."
---

# EnumerationItems

!!! abstract "Collection &middot; `ScriptNavi.chm`"
    Collection: EnumerationItems

Elements of a enumeration in the model of a data store.

## Python example

```python
oMyDataStore = dd.Navigator.ConnectDataStore("ASAM Browse Settings Example")
oMyEnumItems = oMyDataStore.Model.Enumerations.Item(1).Items
print(oMyEnumItems.Count)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itdmenumerationitems-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itdmenumerationitems-exists/">Exists</a> | <a href="../../methods/itdmenumerationitems-item/">Item</a> | <a href="../../methods/itdmenumerationitems-itembyvalue/">ItemByValue</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itdmmodelenumeration/">ModelEnumeration</a>.<a href="../../properties/itdmmodelenumeration-items/">Items</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/Objects/navigator_Objects_ITDMEnumerationItems.htm`*

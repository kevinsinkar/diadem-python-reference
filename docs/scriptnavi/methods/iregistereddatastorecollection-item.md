---
title: "IRegisteredDataStoreCollection.Item"
description: "Returns the connection definition associated with a specific name or a specific index of a registered data store."
---

# IRegisteredDataStoreCollection.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for RegisteredDataStores <Navigator>

Returns the connection definition associated with a specific name or a specific index of a registered data store.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyDataStore = dd.Navigator.Settings.RegisteredDataStores.Item(1)
dd.MsgBoxDisp(oMyDataStore.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IRegisteredDataStoreCollection.htm`*

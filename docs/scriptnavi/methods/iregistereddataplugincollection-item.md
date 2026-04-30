---
title: "IRegisteredDataPluginCollection.Item"
description: "Uses the name or the index to access a DataPlugin registered on your computer."
---

# IRegisteredDataPluginCollection.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for RegisteredDataPlugins <Navigator>

Uses the name or the index to access a DataPlugin registered on your computer.

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the Item method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyRegisteredDataPlugins = dd.Navigator.Settings.RegisteredDataPlugins
dd.MsgBoxDisp (oMyRegisteredDataPlugins.Item(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IRegisteredDataPluginCollection.htm`*

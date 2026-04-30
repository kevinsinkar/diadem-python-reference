---
title: "IUpdateData.Item"
description: "Uses the name or the index to access information about a DataPlugin in the update source."
---

# IUpdateData.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for UpdateData <Navigator>

Uses the name or the index to access information about a DataPlugin in the update source.

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
oMyDataUpdateSource = dd.Navigator.Settings.CreateUpdateSource()
oMyUpdateData = oMyDataUpdateSource.UpdateData
dd.MsgBoxDisp(oMyUpdateData.Item(1).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_IUpdateData.htm`*

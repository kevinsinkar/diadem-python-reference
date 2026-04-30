---
title: "ITDMReturnTypeColumns.Item"
description: "Returns in the search results list the ReturnTypeColumns object which belongs to a certain index."
---

# ITDMReturnTypeColumns.Item

!!! abstract "Method &middot; `ScriptNavi.chm`"
    Method: Item for ReturnTypeColumns

Returns in the search results list the ReturnTypeColumns object which belongs to a certain index.

## Signature

```python
return_value = obj.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMySettings = dd.Navigator.Display.CurrDataFinder.ResultsList.Settings
dd.MsgBoxDisp(oMySettings.Columns(dd.eSearchFile).Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ScriptNavi/methods/navigator_method_Item_ITDMReturnTypeColumns.htm`*

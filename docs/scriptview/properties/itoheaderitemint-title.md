---
title: "IToHeaderItemInt.Title"
description: "Specifies the channel properties in the column header of a channel table in DIAdem VIEW."
---

# IToHeaderItemInt.Title

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Title for HeaderItem

Specifies the channel properties in the column header of a channel table in DIAdem VIEW.

## Signature

```python
obj.Title
```

## Python example

```python
oMyCollection = dd.View.ActiveSheet.ActiveArea.DisplayObj.HeaderItems
for oMyItem in oMyCollection:
    dd.MsgBoxDisp("Title of HeaderItem: " + oMyItem.Title)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Title_IToHeaderItemInt.htm`*

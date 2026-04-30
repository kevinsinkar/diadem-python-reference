---
title: "IToHeaderItemInt"
description: "The HeaderItem object provides access to a table heading for a channel table in DIAdem VIEW. DIAdem displays channel properties in the table titles. DIAdem disp"
---

# IToHeaderItemInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: HeaderItem

The HeaderItem object provides access to a table heading for a channel table in DIAdem VIEW. DIAdem displays channel properties in the table titles. DIAdem displays the property names in the index column.

## Python example

```python
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyHeaders = oMySheet.ActiveArea.DisplayObj.HeaderItems
sOutput  = "List of header items: " + "\r\n"
for HeaderItem in oMyHeaders:
    sOutput = sOutput + HeaderItem.Name + "\r\n"
print(sOutput)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itoheaderitemint-format/">Format</a> | <a href="../../properties/itoheaderitemint-name/">Name</a> | <a href="../../properties/itoheaderitemint-title/">Title</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/headeritems/">HeaderItems</a>.<a href="../../methods/itoheaderitems-add/">Add</a> | <a href="../../collections/headeritems/">HeaderItems</a>.<a href="../../methods/itoheaderitems-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToHeaderItemInt.htm`*

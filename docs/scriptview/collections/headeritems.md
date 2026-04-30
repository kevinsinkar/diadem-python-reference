---
title: "HeaderItems"
description: "The HeaderItems object provides a list of all the table headings in a channel table in the DIAdem VIEW panel. Use the HeaderItems collection to delete table hea"
---

# HeaderItems

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: HeaderItems

The HeaderItems object provides a list of all the table headings in a channel table in the DIAdem VIEW panel. Use the HeaderItems collection to delete table headings or to add new table headings.

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
<p><a href="../../properties/itoheaderitems-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itoheaderitems-add/">Add</a> | <a href="../../methods/itoheaderitems-item/">Item</a> | <a href="../../methods/itoheaderitems-remove/">Remove</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itochanneltableint/">ChannelTable</a>.<a href="../../properties/itochanneltableint-headeritems/">HeaderItems</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToHeaderItems.htm`*

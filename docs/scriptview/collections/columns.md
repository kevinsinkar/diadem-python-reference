---
title: "Columns"
description: "The Columns object provides a collection of the Columns in a channel table in DIAdem VIEW. Use the Columns collection to delete columns or to add new columns."
---

# Columns

!!! abstract "Collection &middot; `Scriptview.chm`"
    Collection: Columns

The Columns object provides a collection of the Columns in a channel table in DIAdem VIEW. Use the Columns collection to delete columns or to add new columns.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The contents of the properties of the Columns collection are only valid if the <a href="../../properties/itochanneltableint-dynamicmode/">DynamicMode</a> property of the ChannelTable object contains the value <span class="Monospace">NONE</span>.</td></tr></table>
</div>

## Python example

```python
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.Name = "MySheet"
oMySheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.Columns.Add("[1]/[1]")
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itochnenumint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itochnenumint-add/">Add</a> | <a href="../../methods/itochnenumint-item/">Item</a> | <a href="../../methods/itochnenumint-remove/">Remove</a> | <a href="../../methods/itochnenumint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/itochanneltableint/">ChannelTable</a>.<a href="../../properties/itochanneltableint-columns/">Columns</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToChnEnumInt.htm`*

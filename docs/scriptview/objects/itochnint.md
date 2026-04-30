---
title: "IToChnInt"
description: "The Column object provides a column in a channel table in DIAdem VIEW. Use the Column object to specify information about this column."
---

# IToChnInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: Column

The Column object provides a column in a channel table in DIAdem VIEW. Use the Column object to specify information about this column.

## Python example

```python
dd.View.Sheets.RemoveAll()
dd.View.NewLayout()
oMySheet = dd.View.ActiveSheet
oMySheet.Name = "MySheet"
oMySheet.ActiveArea.DisplayObjType = "ChannelTable"
oMyChart = oMySheet.ActiveArea.DisplayObj
oMyChart.Columns.Add("[1]/[1]")
oMyChart.Columns.Add("[1]/[2]")
for oColumn in oMyChart.Columns:
    oColumn.Format = "d.dd"
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itochnint-channelname/">ChannelName</a> | <a href="../../properties/itochnint-format/">Format</a> | <a href="../../properties/itochnint-index/">Index</a> | <a href="../../properties/itochnint-name/">Name</a> | <a href="../../properties/itochnint-tagstored/">TagStored</a> | <a href="../../properties/itochnint-tagtemporary/">TagTemporary</a> | <a href="../../properties/itochnint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itochanneltableint/">ChannelTable</a>.<a href="../../properties/itochanneltableint-currcolumn/">CurrColumn</a> | <a href="../../collections/columns/">Columns</a>.<a href="../../methods/itochnenumint-add/">Add</a> | <a href="../../collections/columns/">Columns</a>.<a href="../../methods/itochnenumint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToChnInt.htm`*

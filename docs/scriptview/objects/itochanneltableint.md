---
title: "IToChannelTableInt"
description: "The ChannelTable object provides a channel table in DIAdem VIEW. In the ChannelTable object you display channel values and attributes and edit data."
---

# IToChannelTableInt

!!! abstract "Object &middot; `Scriptview.chm`"
    Object: ChannelTable

The ChannelTable object provides a channel table in DIAdem VIEW. In the ChannelTable object you display channel values and attributes and edit data.

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
<p><a href="../../properties/itochanneltableint-activecolumn/">ActiveColumn</a> | <a href="../../properties/itochanneltableint-activerow/">ActiveRow</a> | <a href="../../properties/itochanneltableint-alignment/">Alignment</a> | <a href="../../properties/itochanneltableint-area/">Area</a> | <a href="../../properties/itochanneltableint-columns/">Columns</a> | <a href="../../properties/itochanneltableint-columnsfrozen/">ColumnsFrozen</a> | <a href="../../properties/itochanneltableint-currcolumn/">CurrColumn</a> | <a href="../../properties/itochanneltableint-cursormode/">CursorMode</a> | <a href="../../properties/itochanneltableint-dynamicmode/">DynamicMode</a> | <a href="../../properties/itochanneltableint-dynamicmodegroupname/">DynamicModeGroupName</a> | <a href="../../properties/itochanneltableint-font/">Font</a> | <a href="../../properties/itochanneltableint-headeritems/">HeaderItems</a> | <a href="../../properties/itochanneltableint-highlight/">Highlight</a> | <a href="../../properties/itochanneltableint-indexcolumnwidth/">IndexColumnWidth</a> | <a href="../../properties/itochanneltableint-numformat/">NumFormat</a> | <a href="../../properties/itochanneltableint-timeformat/">TimeFormat</a> | <a href="../../properties/itochanneltableint-toolbarvisible/">ToolbarVisible</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itochanneltableint-gotoendoflongestcolumn/">GoToEndOfLongestColumn</a> | <a href="../../methods/itochanneltableint-setactivecell/">SetActiveCell</a> | <a href="../../methods/itochanneltableint-showcolumnsdlg/">ShowColumnsDlg</a> | <a href="../../methods/itochanneltableint-showgotodlg/">ShowGoToDlg</a> | <a href="../../methods/itochanneltableint-showprintdlg/">ShowPrintDlg</a> | <a href="../../methods/itochanneltableint-showpropertiesdlg/">ShowPropertiesDlg</a> | <a href="../../methods/itochanneltableint-showsettingsdlg/">ShowSettingsDlg</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../itoareaobjectint/">Area</a>.<a href="../../properties/itoareaobjectint-displayobj/">DisplayObj</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/objects/VIEW_Objects_IToChannelTableInt.htm`*

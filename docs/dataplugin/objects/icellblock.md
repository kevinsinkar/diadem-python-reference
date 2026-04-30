---
title: "ICellBlock"
description: "The CellBlock object makes accessing data in a workbook easier. A CellBlock can contain one or more DirectAccess channels. The channel values are organized colu"
---

# ICellBlock

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: CellBlock

The CellBlock object makes accessing data in a workbook easier. A CellBlock can contain one or more DirectAccess channels. The channel values are organized columnwise in this block. You read the contents of a workbook as follows: - use the Workbook.GetCellBlock method and assign the return value to a variable. - add a DirectAccess channel to the CellBlock for each channel to be read, - assign the complete DirectAccess channel to a channel group. Note The file pointer of the worksheet does not move when a CellBlock is read out.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The file pointer of the worksheet does not move when a CellBlock is read out.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(2,1)

for i in range(1, oCurrSheet.MaxPosition.Column + 1):
    Name = oCurrSheet.GetCellValue(1,i)
    oNewChannel = oCellBlock.Channels.Add(Name)
    Root.ChannelGroups(1).Channels.AddDirectAccessChannel(oNewChannel)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icellblock-blocklength/">BlockLength</a> | <a href="../../properties/icellblock-channels/">Channels</a> | <a href="../../properties/icellblock-position/">Position</a></p>
</div>
<div class="Methods">
<h2>Returned From</h2>
<p><a href="../iexcelsheet/">Sheet</a>.<a href="../../methods/iexcelsheet-getcellblock/">GetCellBlock</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_ICellBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "ICellBlock.BlockLength"
description: "Specifies the number of values that a channel in the CellBlock contains. If the number is -1 , the block extends to the end of the file."
---

# ICellBlock.BlockLength

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: BlockLength for CellBlock

Specifies the number of values that a channel in the CellBlock contains. If the number is -1 , the block extends to the end of the file.

## Signature

```python
obj.BlockLength
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(2,1)
oCellBlock.BlockLength = 5

for i in range(1, oCurrSheet.MaxPosition.Column + 1):
    Name = oCurrSheet.GetCellValue(1,i)
    oNewChannel = oCellBlock.Channels.Add(Name)
    Root.ChannelGroups(1).Channels.AddDirectAccessChannel(oNewChannel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_BlockLength_ICellBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

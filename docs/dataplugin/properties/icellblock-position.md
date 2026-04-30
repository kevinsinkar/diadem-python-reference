---
title: "ICellBlock.Position"
description: "Specifies the position of the file pointer in a CellBlock."
---

# ICellBlock.Position

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Position for CellBlock

Specifies the position of the file pointer in a CellBlock.

## Signature

```python
return_value = obj.Position
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(4,1)

for i in range(oCellBlock.Position.Column, oCurrSheet.MaxPosition.Column + 1):
    Name = oCurrSheet.GetCellValue(oCellBlock.Position.Row-1,i)
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

*Source: `DataPlugin/Properties/DataPlugin_property_Position_ICellBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

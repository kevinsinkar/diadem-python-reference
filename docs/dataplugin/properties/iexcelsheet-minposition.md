---
title: "IExcelSheet.MinPosition"
description: "Specifies within the worksheet the position of the cell that contains the first value."
---

# IExcelSheet.MinPosition

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: MinPosition for Sheet

Specifies within the worksheet the position of the cell that contains the first value.

## Signature

```python
return_value = obj.MinPosition
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(oCurrSheet.MinPositiom.Row+1,oCurrSheet.MinPosition.Column)

for i in range(oCurrSheet.MinPosition.Column, oCurrSheet.MaxPosition.Column + 1):
    Name = oCurrSheet.GetCellValue(oCurrSheet.MinPositiom.Row,i)
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

*Source: `DataPlugin/Properties/DataPlugin_property_MinPosition_IExcelSheet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

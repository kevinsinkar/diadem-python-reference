---
title: "IExcelSheet.MaxPosition"
description: "Specifies within the worksheet the position of the cell that contains the last value."
---

# IExcelSheet.MaxPosition

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: MaxPosition for Sheet

Specifies within the worksheet the position of the cell that contains the last value.

## Signature

```python
return_value = obj.MaxPosition
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_MaxPosition_IExcelSheet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

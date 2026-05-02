---
title: "IExcelSheet.GetCellBlock"
description: "Reads the worksheet starting at a specified position and returns the channel values the worksheet contains."
---

# IExcelSheet.GetCellBlock

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetCellBlock for Sheet

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Reads the worksheet starting at a specified position and returns the channel values the worksheet contains.

## Signature

```python
return_value = obj.GetCellBlock(Row, Column, [Direction])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDirectionVertical` | 1 | Columnwise |
| `eDirectionHorizontal` | 2 | Rowwise |

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

*Source: `DataPlugin/Methods/DataPlugin_method_GetCellBlock_IExcelSheet.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

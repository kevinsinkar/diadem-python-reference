---
title: "IExcelPosition.Column"
description: "Specifies the column number of a cell in a worksheet."
---

# IExcelPosition.Column

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Column for CellPosition

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the column number of a cell in a worksheet.

## Signature

```python
obj.Column
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(1,1)

for i in range(1, oCurrSheet.MaxPosition.Column + 1):
    oNewChannel = oCellBlock.Channels.Add("ExcelRow_"&i)
    Root.ChannelGroups(1).Channels.AddDirectAccessChannel(oNewChannel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Column_IExcelPosition.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

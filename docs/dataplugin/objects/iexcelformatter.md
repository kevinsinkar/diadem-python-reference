---
title: "IExcelFormatter"
description: "The CellFormatter object contains information about the format of the workbook that the DataPlugin is currently processing."
---

# IExcelFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: CellFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The CellFormatter object contains information about the format of the workbook that the DataPlugin is currently processing.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oCurrSheet = Workbook.Sheets(1)
oCellBlock = oCurrSheet.GetCellBlock(1,1)
Workbook.Formatter.NoValueSign = "NV"

for i in range(1, oCurrSheet.MaxPosition.Column + 1):
    oNewChannel = oCellBlock.Channels.Add("Excel_Row"&i)
    Root.ChannelGroups(1).Channels.AddDirectAccessChannel(oNewChannel)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iexcelformatter-novaluesign/">NoValueSign</a> | <a href="../../properties/iexcelformatter-timeformat/">TimeFormat</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../iexcelfileio/">Workbook</a>.<a href="../../properties/iexcelfileio-formatter/">Formatter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IExcelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

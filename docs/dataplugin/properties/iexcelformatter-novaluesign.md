---
title: "IExcelFormatter.NoValueSign"
description: "Specifies the NoValue character used in the workbook."
---

# IExcelFormatter.NoValueSign

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: NoValueSign for CellFormatter

Specifies the NoValue character used in the workbook.

## Signature

```python
obj.NoValueSign
```

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

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_NoValueSign_IExcelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

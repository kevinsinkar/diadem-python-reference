---
title: "DirectCellChannels"
description: "Collection of all DirectAccess channels. You can use the DirectCellChannels collection to delete or to add DirectAccess channels."
---

# DirectCellChannels

!!! abstract "Collection &middot; `DataPlugin.chm`"
    Collection: DirectCellChannels

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Collection of all DirectAccess channels. You can use the DirectCellChannels collection to delete or to add DirectAccess channels.

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
<p><a href="../../properties/iexceldachannels-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iexceldachannels-add/">Add</a> | <a href="../../methods/iexceldachannels-item/">Item</a> | <a href="../../methods/iexceldachannels-remove/">Remove</a> | <a href="../../methods/iexceldachannels-removeall/">RemoveAll</a> | <a href="../../methods/iexceldachannels-swap/">Swap</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/icellblock/">CellBlock</a>.<a href="../../properties/icellblock-channels/">Channels</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IExcelDAChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "ICellChannelFormatter"
description: "The CellChannelFormatter object contains information about how the values of a channel are represented in the workbook."
---

# ICellChannelFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: CellChannelFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The CellChannelFormatter object contains information about how the values of a channel are represented in the workbook.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in oBlock.Channels:
    if (oMyChn.Formatter.IsKindOf(eCellBlock)):
        oMyChn.Properties.Add("DataType", oMyChn.Formatter.DataType)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/icellchannelformatter-block/">Block</a> | <a href="../../properties/icellchannelformatter-datatype/">DataType</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/icellchannelformatter-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idirectaccesschannel/">DirectAccessChannel</a>.<a href="../../properties/idirectaccesschannel-formatter/">Formatter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_ICellChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

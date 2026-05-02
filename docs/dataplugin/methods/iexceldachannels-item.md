---
title: "IExcelDAChannels.Item"
description: "Returns the DirectAccessChannel object associated with a specific name or with a specific index."
---

# IExcelDAChannels.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for DirectCellChannels

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the DirectAccessChannel object associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(DAChnNameOrIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, oCellBlock.Channels.Count + 1):
    ChannelGroup.Channels.AddDirectAccessChannel(oCellBlock.Channels.Item(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IExcelDAChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

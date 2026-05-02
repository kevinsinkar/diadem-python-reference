---
title: "IChannelsToProcess.Item"
description: "Returns the Channel object of a specific index."
---

# IChannelsToProcess.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for ChannelsToProcess

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Returns the Channel object of a specific index.

## Signature

```python
return_value = obj.Item(iIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for i in range(1, ProcessedChn.Channels.Count + 1):
    ProcessedChn.Properties.Add(ProcessedChn.Channels.Item(i).Name,"Composite")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IChannelsToProcess.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

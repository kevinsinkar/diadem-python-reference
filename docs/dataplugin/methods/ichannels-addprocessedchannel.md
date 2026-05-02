---
title: "IChannels.AddProcessedChannel"
description: "Adds an object to the Channels collection and returns a ProcessedChannel object."
---

# IChannels.AddProcessedChannel

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddProcessedChannel for Channels <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Adds an object to the Channels collection and returns a ProcessedChannel object.

## Signature

```python
return_value = obj.AddProcessedChannel(NameOrChannel, eProcessingType, ProcessingType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The channel name must be unique and must not include special characters.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oChannelGroup = Root.ChannelGroups("Measurements")
oProcessedChn = oChannelGroup.Channels.AddProcessedChannel("MyChannel",eR64,eAddProcessor)
for i in range(2, 4 + 1):
    oProcessedChn.Channels.Add(oChannelGroup.Channels(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddProcessedChannel_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

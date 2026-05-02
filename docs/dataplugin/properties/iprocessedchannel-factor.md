---
title: "IProcessedChannel.Factor"
description: "Specifies the factor that the read value is multiplied by."
---

# IProcessedChannel.Factor

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Factor for ProcessedChannel

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the factor that the read value is multiplied by.

## Signature

```python
obj.Factor
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  The properties <span class="Monospace">Factor</span> and <span class="Monospace">Offset</span> are ignored when text channels and time channels are read. For all other channel types, the conversion formula returns a Real result.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oChannelGroup = Root.ChannelGroups("Measurements")
oProcessedChn = oChannelGroups.Channels.AddProcessedChannel("MyChannel",eR64,eAddProcessor)
oProcessedChn.Factor = 2
oProcessedChn.Offset = 5
for i in range(2, 4 + 1):
    oProcessedChn.Channels.Add(oChannelGroup.Channels(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Factor_IProcessedChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

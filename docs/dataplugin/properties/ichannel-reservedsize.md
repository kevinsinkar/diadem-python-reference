---
title: "IChannel.ReservedSize"
description: "Specifies the number of values that are reserved for a channel."
---

# IChannel.ReservedSize

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: ReservedSize for Channel <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the number of values that are reserved for a channel.

## Signature

```python
obj.ReservedSize
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
File.Formatter.Delimiters = ";"
File.Formatter.TimeFormat = "DD.MM.YYYY hh:mm:ss"
oMyChn.ReservedSize = ChannelSize
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_ReservedSize_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

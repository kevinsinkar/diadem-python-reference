---
title: "IChannels.AddImplicitChannel"
description: "Adds an object to the Channels collection and returns an ImplicitChannel object."
---

# IChannels.AddImplicitChannel

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddImplicitChannel for Channels <DataPlugin>

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Adds an object to the Channels collection and returns an ImplicitChannel object.

## Signature

```python
return_value = obj.AddImplicitChannel(sName, StartValue, Increment, Size, eDataType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The channel name must be unique and must not include special characters.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The parameters <em>StartValue</em> and <em>Increment</em> must be the same data type.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eI16` | 2 | 16-bit integer values |
| `eI32` | 3 | 32-bit integer values |
| `eR32` | 9 | 32-bit real values |
| `eR64` | 10 | 64-bit real values |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyGrp = Root.ChannelGroups.Add("MyChnGroup")
oMyGrp.Channels.AddImplicitChannel("Implchannel", 0, 10, 100, eI32)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddImplicitChannel_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

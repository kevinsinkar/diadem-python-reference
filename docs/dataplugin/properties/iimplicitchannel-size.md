---
title: "IImplicitChannel.Size"
description: "Specifies the number of values of an implicit channel."
---

# IImplicitChannel.Size

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Size for ImplicitChannel

Specifies the number of values of an implicit channel.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if ChannelType = "eI32":
    ChannelGroup.Channels.AddImplicitChannel(ChannelName, StartValue, Increment, ChannelSize, eI32)
else:
    RaiseError("InvalidTypeString " + ChannelType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Size_IImplicitChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IChannel.Size"
description: "Returns the current number of values in a channel."
---

# IChannel.Size

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Size for Channel <DataPlugin>

Returns the current number of values in a channel.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
bIndexChn = FALSE
for oMyChn in Root.ChannelGroups(1).Channels:
    if (oMyChn.Name=="MyChannel") and not bIndexChn:
        bIndexChn = TRUE
        Root.ChannelGroups(1).Channels.AddImplicitChannel("Index", 1, 1, oMyChn.Size, eI32)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Size_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

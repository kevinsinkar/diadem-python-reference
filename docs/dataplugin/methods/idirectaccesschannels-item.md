---
title: "IDirectAccessChannels.Item"
description: "Returns the DirectAccessChannel object associated with a specific name or with a specific index."
---

# IDirectAccessChannels.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for DirectAccessChannels

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
for i in range(1, oBlock.Channels.Count + 1):
    ChannelGroup.Channels.AddDirectAccessChannel(oBlock.Channels.Item(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IDirectAccessChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

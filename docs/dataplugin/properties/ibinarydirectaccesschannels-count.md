---
title: "IBinaryDirectAccessChannels.Count"
description: "Returns the number of elements in a BinaryDirectAccessChannels collection."
---

# IBinaryDirectAccessChannels.Count

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Count for BinaryDirectAccessChannels

Returns the number of elements in a BinaryDirectAccessChannels collection.

## Signature

```python
obj.Count
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oBlock.Channels.Add("Channel1",eI32)
oBlock.Channels.Add("Channel2",eI32)
for i in range(1, oBlock.Channels.Count + 1):
    ChannelGroup.Channels.AddDirectAccessChannel(Block.Channels.Item(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Count_IBinaryDirectAccessChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

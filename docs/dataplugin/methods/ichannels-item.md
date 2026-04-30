---
title: "IChannels.Item"
description: "Returns the Channel object associated with a specific name or with a specific index."
---

# IChannels.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for Channels <DataPlugin>

Returns the Channel object associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(ChnNameorIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyGrp = Root.ChannelGroups.Item("FirstChnGroup")
oMyChn = oMyGrp.Channels.Item(3)
if oMyChn.IsKindOf(eImplicit):
    oMyChn.Properties.Add("Offset",-5)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IChannels.AddStoreChannel"
description: "Adds an object to the Channels collection and returns an ImplicitChannel object or a ProcessedChannel object."
---

# IChannels.AddStoreChannel

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: AddStoreChannel for Channels <DataPlugin>

Adds an object to the Channels collection and returns an ImplicitChannel object or a ProcessedChannel object.

## Signature

```python
return_value = obj.AddStoreChannel(oChannel, [sName])
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
def ReadStore(FromStore):
    FindAndCreateGroups(FromStore.Children)

def FindAndCreateGroups(StoreElements):
    for StoreElement in StoreElements:
        if StoreElement.IsKindOf(eStoreChannelGroup):
            TDMGroup = Root.ChannelGroups.Add(StoreElement.Name)
            TDMGroup.Properties.AddProperties(StoreElement.Properties)
            CreateChannels(StoreElement, TDMGroup)
        else:
            FindAndCreateGroups(StoreElement.Children)

def CreateChannels(StoreGroup, TDMGroup):
    for StoreChannel in StoreGroup.Channels:
        TDMGroup.Channels.AddStoreChannel(StoreChannel)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_AddStoreChannel_IChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

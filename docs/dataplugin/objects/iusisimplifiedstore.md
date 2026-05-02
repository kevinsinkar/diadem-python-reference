---
title: "IUSISimplifiedStore"
description: "The Store object provides information on the data store currently processed by the DataPlugin. Use the Store object properties to specify how to map the informa"
---

# IUSISimplifiedStore

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Store

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

The Store object provides information on the data store currently processed by the DataPlugin. Use the Store object properties to specify how to map the information about a data model, for example, ATFX files, onto the TDM data model. You also can use the Store object to change, to rename, or to extend information about a TDM data model.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iusisimplifiedstore-children/">Children</a> | <a href="../../properties/iusisimplifiedstore-configfilename/">ConfigFileName</a> | <a href="../../properties/iusisimplifiedstore-fileinfo/">FileInfo</a> | <a href="../../properties/iusisimplifiedstore-parameters/">Parameters</a> | <a href="../../properties/iusisimplifiedstore-pluginname/">PluginName</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idataplugin/">DataPlugin</a>.<a href="../../methods/idataplugin-openstore/">OpenStore</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IUSISimplifiedStore.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IUSIElement"
description: "The Element object contains information about the currently edited data store."
---

# IUSIElement

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Element <DataPlugin>

The Element object contains information about the currently edited data store.

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
        else:
            FindAndCreateGroups(StoreElement.Children)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iusielement-children/">Children</a> | <a href="../../properties/iusielement-name/">Name</a> | <a href="../../properties/iusielement-properties/">Properties</a> | <a href="../../properties/iusielement-type/">Type</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iusielement-iskindof/">IsKindOf</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/elements/">Elements &lt;DataPlugin&gt;</a>.<a href="../../methods/iusielements-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IUSIElement.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IUSIElement.Properties"
description: "Contains the Properties collection associated with an Element object."
---

# IUSIElement.Properties

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Properties for Element <DataPlugin>

Contains the Properties collection associated with an Element object.

## Signature

```python
return_value = obj.Properties
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
        else:
            FindAndCreateGroups(StoreElement.Children)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Properties_IUSIElement.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

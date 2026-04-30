---
title: "IUSIElement.Type"
description: "Returns the type of an Element object."
---

# IUSIElement.Type

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Type for Element <DataPlugin>

Returns the type of an Element object.

## Signature

```python
obj.Type
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for j in range(1, FromStore.Children.Count + 1):
    if FromStore.Children.Item(j).IsKindOf(eStoreChannelGroup):
        Root.Properties.AddProperties(StoreElement.Properties, StoreElement.Type + i + "_")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Type_IUSIElement.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

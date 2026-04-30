---
title: "IUSIElements.Item"
description: "Returns the Element object of a specific index."
---

# IUSIElements.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for Elements <DataPlugin>

Returns the Element object of a specific index.

## Signature

```python
return_value = obj.Item(iIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for j in range(1, FromStore.Children.Count + 1):
    if StoreElement.IsKindOf(eStoreChannelGroup):
        Root.Properties.Add("Composite"& right("0"&j,2), FromStore.Children.Item(j).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IUSIElements.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IProperties.Item"
description: "Returns the Property object associated with a specific name or with a specific index."
---

# IProperties.Item

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Item for Properties <DataPlugin>

Returns the Property object associated with a specific name or with a specific index.

## Signature

```python
return_value = obj.Item(PropNameOrIndex)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oMyProp = Root.Properties.Item("Description")
oMyProp.Value = "Example"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Item_IProperties.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

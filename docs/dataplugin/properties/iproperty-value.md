---
title: "IProperty.Value"
description: "Specifies the value of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object."
---

# IProperty.Value

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Value for Property <DataPlugin>

Specifies the value of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object.

## Signature

```python
obj.Value
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyProp in Root.Properties:
    if not oMyProp.Default:
        oMyProp.Value = ""
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Value_IProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

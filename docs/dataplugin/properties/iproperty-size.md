---
title: "IProperty.Size"
description: "Specifies the number of values of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object."
---

# IProperty.Size

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Size for Property <DataPlugin>

Specifies the number of values of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oProp = FromChn.Properties("VectorProperty")
for i in range(1, oProp.Size + 1):
    ToChn.Properties.Add("Prop"&i, oProp.Values(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Size_IProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

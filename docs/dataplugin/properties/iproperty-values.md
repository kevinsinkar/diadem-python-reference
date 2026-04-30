---
title: "IProperty.Values"
description: "Specifies a vector with values of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object. The size o"
---

# IProperty.Values

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Values for Property <DataPlugin>

Specifies a vector with values of a property of the Root object, of the ChannelGroup object, of the Channel object, or of the ImplicitChannel object. The size of the vector depends on the Size property.

## Signature

```python
obj.Values(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>A property only can have several values when this property belongs to an <a href="../../collections/elements/">Element</a> object.</td></tr></table>
</div>

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

*Source: `DataPlugin/Properties/DataPlugin_property_Values_IProperty.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

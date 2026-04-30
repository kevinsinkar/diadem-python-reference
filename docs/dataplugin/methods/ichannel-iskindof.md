---
title: "IChannel.IsKindOf"
description: "Checks whether a Channel object is a certain type."
---

# IChannel.IsKindOf

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: IsKindOf for Channel <DataPlugin>

Checks whether a Channel object is a certain type.

## Signature

```python
iIsKindOf = Object.IsKindOf(Type)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oChn in Root.ChannelGroups(1).Channels:
    if oChn.IsKindOf(eImplicit):
        oChn.Properties.Add("Offset",-5)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_IsKindOf_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

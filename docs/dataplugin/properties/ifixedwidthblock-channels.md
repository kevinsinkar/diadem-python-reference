---
title: "IFixedWidthBlock.Channels"
description: "Contains the DirectAccessChannels collection associated with a FixedWidthBlock object."
---

# IFixedWidthBlock.Channels

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Channels for FixedWidthBlock

Contains the DirectAccessChannels collection associated with a FixedWidthBlock object.

## Signature

```python
return_value = obj.Channels
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
# further instructions
for i in range(1, oBlock.Channels.Count + 1):
    oBlock.Channels(i).Properties.Add("Offset",3)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Channels_IFixedWidthBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

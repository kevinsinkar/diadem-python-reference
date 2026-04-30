---
title: "IStringBlock.Channels"
description: "Contains the DirectAccessChannels collection associated with a StringBlock object."
---

# IStringBlock.Channels

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Channels for StringBlock

Contains the DirectAccessChannels collection associated with a StringBlock object.

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
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Channels_IStringBlock.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

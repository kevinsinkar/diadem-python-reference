---
title: "IChannelGroups.Exists"
description: "Checks whether a ChannelGroup object with a specific name exists."
---

# IChannelGroups.Exists

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Exists for ChannelGroups <DataPlugin>

Checks whether a ChannelGroup object with a specific name exists.

## Signature

```python
iExists = Object.Exists(sName)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
if Root.ChannelGroups.Exists("FirstChnGroup"):
    Root.ChannelGroups.Add("SecondChnGroup")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Exists_IChannelGroups.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IChannelGroups.Add"
description: "Adds an object to the ChannelGroups collection and returns a ChannelGroup object."
---

# IChannelGroups.Add

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Add for ChannelGroups <DataPlugin>

Adds an object to the ChannelGroups collection and returns a ChannelGroup object.

## Signature

```python
return_value = obj.Add(sName)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The name of the channel group must be unique and must not include special characters.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
Root.ChannelGroups.RemoveAll()
Root.ChannelGroups.Add("MyChnGroup")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Add_IChannelGroups.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

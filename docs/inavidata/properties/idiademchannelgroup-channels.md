---
title: "IDiademChannelGroup.Channels"
description: "Contains the Channels collection associated with a ChannelGroup object in the script interface for internal data."
---

# IDiademChannelGroup.Channels

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Channels for ChannelGroup <Data>

Contains the Channels collection associated with a ChannelGroup object in the script interface for internal data.

## Signature

```python
return_value = obj.Channels
```

## Python example

```python
for oMyChn in dd.Data.Root.ChannelGroups(1).Channels:
    oMyChn.Properties.Add("Sensor_Type","TC-N")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Channels_IDiademChannelGroup.HTM`*

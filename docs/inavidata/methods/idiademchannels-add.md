---
title: "IDiademChannels.Add"
description: "Creates a new channel in the script interface for internal data and adds the channel to the Channels collection. The Add method returns a Channel object."
---

# IDiademChannels.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for Channels <Data>

Creates a new channel in the script interface for internal data and adds the channel to the Channels collection. The Add method returns a Channel object.

## Signature

```python
return_value = obj.Add(Name, DataType, [DestIndex])
```

## Python example

```python
oGroupChns = dd.Data.Root.ChannelGroups(1).Channels

if not oGroupChns.Exists("MyChnName") :
    oMyChn = oGroupChns.Add("MyChnName",dd.DataTypeChnFloat64)
else:
    oMyChn = oGroupChns("MyChnName")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2><p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p></div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_IDiademChannels.HTM`*

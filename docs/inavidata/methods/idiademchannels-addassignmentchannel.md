---
title: "IDiademChannels.AddAssignmentChannel"
description: "Creates a new assignment channel in the script interface for internal data."
---

# IDiademChannels.AddAssignmentChannel

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: AddAssignmentChannel for Channels <Data>

Creates a new assignment channel in the script interface for internal data.

## Signature

```python
return_value = obj.AddAssignmentChannel(Name, DefaultValue, [DataType], [DestIndex])
```

## Python example

```python
oGrp = dd.Data.Root.ChannelGroups.Add("MyChnGrp")
oChn = oGrp.Channels.AddAssignmentChannel("MyAssignmentChn", "Default Value")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_AddAssignmentChannel_IDiademChannels.htm`*

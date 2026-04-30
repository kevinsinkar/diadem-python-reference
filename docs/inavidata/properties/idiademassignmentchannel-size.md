---
title: "IDiademAssignmentChannel.Size"
description: "Returns the number of values currently used for an assignment channel, in the script interface for internal data. DIAdem automatically adjusts the value of the "
---

# IDiademAssignmentChannel.Size

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Size for AssignmentChannel <Data>

Returns the number of values currently used for an assignment channel, in the script interface for internal data. DIAdem automatically adjusts the value of the Size property if you write more values to the channel.

## Signature

```python
obj.Size
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
dd.MsgBoxDisp("Name: " + oMyChn.Name + "\r\n" + "Size: " + oMyChn.Size)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Size_IDiademAssignmentChannel.htm`*

---
title: "IDiademAssignmentChannel.ReservedSize"
description: "Specifies the number of values that DIAdem reserves for an assignment channel, in the script interface for internal data. DIAdem automatically adjusts the value"
---

# IDiademAssignmentChannel.ReservedSize

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: ReservedSize for AssignmentChannel <Data>

Specifies the number of values that DIAdem reserves for an assignment channel, in the script interface for internal data. DIAdem automatically adjusts the value of the ReservedSize property if an assignment channel requires more values than specified.

## Signature

```python
obj.ReservedSize
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
dd.MsgBoxDisp("Reserved Size: " + oMyChn.ReservedSize)
oMyChn.dValues[10] = 15
dd.MsgBoxDisp("Value(10) = " +  oMyChn.dValues(10) + "\r\n" + "Reserved Size = " + oMyChn.ReservedSize)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_ReservedSize_IDiademAssignmentChannel.htm`*

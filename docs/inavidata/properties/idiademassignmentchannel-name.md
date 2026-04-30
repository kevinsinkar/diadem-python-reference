---
title: "IDiademAssignmentChannel.Name"
description: "Specifies the name of an assignment channel in the script interface for internal data."
---

# IDiademAssignmentChannel.Name

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Name for AssignmentChannel <Data>

Specifies the name of an assignment channel in the script interface for internal data.

## Signature

```python
obj.Name
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
dd.MsgBoxDisp(oMyChn.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Name_IDiademAssignmentChannel.htm`*

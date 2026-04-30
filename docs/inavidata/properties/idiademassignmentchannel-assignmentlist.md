---
title: "IDiademAssignmentChannel.AssignmentList"
description: "Specifies the list of assignments of an assignment channel in the script interface for internal data."
---

# IDiademAssignmentChannel.AssignmentList

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: AssignmentList for AssignmentChannel <Data>

Specifies the list of assignments of an assignment channel in the script interface for internal data.

## Signature

```python
return_value = obj.AssignmentList
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value", dd.DataTypeChnFloat64, 1)
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",10)
oMyAssgnList.Add("text2",20)
oMyAssgnList.Add("text3",30)
for Assignment in oMyAssgnList:
    dd.MsgBoxDisp("Definition Value: " + Assignment.Definition + "\r\n" + "Text Value: " + Assignment.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_AssignmentList_IDiademAssignmentChannel.htm`*

---
title: "IAssignmentList.Count"
description: "Returns the number of assignments in the assignment list of an assignment channel in the script interface for internal data."
---

# IAssignmentList.Count

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Count for AssignmentList <Data>

Returns the number of assignments in the assignment list of an assignment channel in the script interface for internal data.

## Signature

```python
obj.Count
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
dd.MsgBoxDisp(oMyAssgnList.Count)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Count_IAssignmentList.htm`*

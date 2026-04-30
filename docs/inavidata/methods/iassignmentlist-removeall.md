---
title: "IAssignmentList.RemoveAll"
description: "Deletes all assignments of an assignment channel in the script interface for internal data."
---

# IAssignmentList.RemoveAll

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: RemoveAll for AssignmentList <Data>

Deletes all assignments of an assignment channel in the script interface for internal data.

## Signature

```python
obj.RemoveAll()
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyAssignChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyAssignChn.AssignmentList
oMyAssignChn.AssignmentList.Add("text1",[0,1])
oMyAssignChn.AssignmentList.Add("text2",[2,3])
oMyAssignChn.AssignmentList.Add("text3",[4,5])
oMyAssgnList.RemoveAll()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_RemoveAll_IAssignmentList.htm`*

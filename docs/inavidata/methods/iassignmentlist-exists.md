---
title: "IAssignmentList.Exists"
description: "Checks in the script interface for internal data whether an assignment with the specified text value already exists in an assignment channel."
---

# IAssignmentList.Exists

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Exists for AssignmentList <Data>

Checks in the script interface for internal data whether an assignment with the specified text value already exists in an assignment channel.

## Signature

```python
bExists = Object.Exists(Value)
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
dd.MsgBoxDisp(oMyAssgnList.Exists("text2"))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Exists_IAssignmentList.htm`*

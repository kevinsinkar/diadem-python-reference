---
title: "IAssignmentList.Add"
description: "Creates a new assignment in the assignment list of an assignment channel in the script interface for internal data ."
---

# IAssignmentList.Add

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: Add for AssignmentList <Data>

Creates a new assignment in the assignment list of an assignment channel in the script interface for internal data .

## Signature

```python
return_value = obj.Add(Value, Definition)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>DIAdem always orders the list of assignments in the ascending order of the <span class="Monospace">Definition</span> property. If you used the methods <a href="./">Add</a> or <a href="../iassignmentlist-remove/">Remove</a> to change the list of assignments, the index no longer corresponds with the previous position of the assignment in the list.</td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value", dd.DataTypeChnFloat64, 1)
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
for Assignment in oMyAssgnList:
    dd.MsgBoxDisp("Definition Value: " + Assignment.Definition + "\r\n" + "Text: " + Assignment.Value)
```

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value", dd.DataTypeChnFloat64, 1)
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",[1,2])
oMyAssgnList.Add("text2",[3,4])
oMyAssgnList.Add("text3",[5,6])
for Assignment in oMyAssgnList:
    vRange = Assignment.DefinitionRange
    dd.MsgBoxDisp("Definition Range " + vRange(0) + " - " + vRange(1) + ": " + Assignment.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_Add_IAssignmentList.htm`*

---
title: "IAssignment"
description: "The assignment object provides an individual assignment of an assignment channel in the script interface for internal data. A text value (property Value ) is as"
---

# IAssignment

!!! abstract "Object &middot; `Inavidata.chm`"
    Object: Assignment <Data>

The assignment object provides an individual assignment of an assignment channel in the script interface for internal data. A text value (property Value ) is assigned to a numeric value (property Definition ) or to a value range (property DefinitionRange ) in order to define an assignment.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note</strong>  Assignment channels do not support assignments to time values.</td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value", dd.DataTypeChnFloat64, 1)
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",[10,20])
oMyAssgnList.Add("text2",[30,40])
oMyAssgnList.Add("text3",[50,60])
for Assignment in oMyAssgnList:
    vRange = Assignment.DefinitionRange
    dd.MsgBoxDisp("Definition Range " + vRange(0) + " - " + vRange(1) + ": " + Assignment.Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iassignment-definition/">Definition</a> | <a href="../../properties/iassignment-definitionrange/">DefinitionRange</a> | <a href="../../properties/iassignment-value/">Value</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/assignmentlist/">AssignmentList &lt;Data&gt;</a>.<a href="../../methods/iassignmentlist-add/">Add</a> | <a href="../../collections/assignmentlist/">AssignmentList &lt;Data&gt;</a>.<a href="../../methods/iassignmentlist-findbydefinition/">FindByDefinition</a> | <a href="../../collections/assignmentlist/">AssignmentList &lt;Data&gt;</a>.<a href="../../methods/iassignmentlist-findbyvalue/">FindByValue</a> | <a href="../../collections/assignmentlist/">AssignmentList &lt;Data&gt;</a>.<a href="../../methods/iassignmentlist-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IAssignment.htm`*

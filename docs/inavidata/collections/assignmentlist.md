---
title: "AssignmentList"
description: "Collection of the assignments of an assignment channel in the script interface for internal data."
---

# AssignmentList

!!! abstract "Collection &middot; `Inavidata.chm`"
    Collection: AssignmentList <Data>

Collection of the assignments of an assignment channel in the script interface for internal data.

## Python example

```python
chn = dd.Data.Root.ChannelGroups(1).Channels.AddAssignmentChannel("MyAssignmentChn", "Default Value")
chn.AssignmentList.Add("text1", [1, 2])
chn.AssignmentList.Add("text2", [3, 4])
chn.AssignmentList.Add("text3", [5, 6])
for assignment in chn.AssignmentList:
    range = assignment.DefinitionRange
    print("Range", range[0], "-", range[1], ":", assignment.Value)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iassignmentlist-boundarylimitsleft/">BoundaryLimitsLeft</a> | <a href="../../properties/iassignmentlist-boundarylimitsright/">BoundaryLimitsRight</a> | <a href="../../properties/iassignmentlist-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iassignmentlist-add/">Add</a> | <a href="../../methods/iassignmentlist-exists/">Exists</a> | <a href="../../methods/iassignmentlist-existsbydefinition/">ExistsByDefinition</a> | <a href="../../methods/iassignmentlist-findbydefinition/">FindByDefinition</a> | <a href="../../methods/iassignmentlist-findbyvalue/">FindByValue</a> | <a href="../../methods/iassignmentlist-item/">Item</a> | <a href="../../methods/iassignmentlist-remove/">Remove</a> | <a href="../../methods/iassignmentlist-removeall/">RemoveAll</a> | <a href="../../methods/iassignmentlist-setboundarylimits/">SetBoundaryLimits</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/idiademassignmentchannel/">AssignmentChannel &lt;Data&gt;</a>.<a href="../../properties/idiademassignmentchannel-assignmentlist/">AssignmentList</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/objects/DiaCmpnt_Objects_IAssignmentList.htm`*

---
title: "IAssignmentList.FindByDefinition"
description: "Uses the value to determine an assignment of texts to values in the script interface for internal data."
---

# IAssignmentList.FindByDefinition

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: FindByDefinition for AssignmentList <Data>

Uses the value to determine an assignment of texts to values in the script interface for internal data.

## Signature

```python
return_value = obj.FindByDefinition(Definition)
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
dd.MsgBoxDisp(oMyAssgnList.FindByDefinition(2).Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_FindByDefinition_IAssignmentList.htm`*

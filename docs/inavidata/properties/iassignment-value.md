---
title: "IAssignment.Value"
description: "Specifies the text value of an assignment in an assignment channel in the script interface for internal data. A text value (property Value ) is assigned to a nu"
---

# IAssignment.Value

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Value for Assignment <Data>

Specifies the text value of an assignment in an assignment channel in the script interface for internal data. A text value (property Value ) is assigned to a numeric value (property Definition ) or to a value range (property DefinitionRange) in order to define an assignment.

## Signature

```python
obj.Value
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
for Assignment in oMyAssgnList:
    dd.MsgBoxDisp("Definition Value: " + Assignment.Definition + "\r\n" + "Text: " + Assignment.Value)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Value_IAssignment.htm`*

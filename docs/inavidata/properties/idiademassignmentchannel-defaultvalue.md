---
title: "IDiademAssignmentChannel.DefaultValue"
description: "Specifies the default text of an assignment channel in the script interface for internal data. DIAdem displays this default text when all the specified assignme"
---

# IDiademAssignmentChannel.DefaultValue

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: DefaultValue for AssignmentChannel <Data>

Specifies the default text of an assignment channel in the script interface for internal data. DIAdem displays this default text when all the specified assignments are invalid.

## Signature

```python
obj.DefaultValue
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value", dd.DataTypeChnFloat64, 1)
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("Text1",[10,20])
oMyAssgnList.Add("Text2",[30,40])
oMyAssgnList.Add("Text3",[50,60])
dd.MsgBoxDisp("Channel default value: " + oMyChn.DefaultValue)
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

*Source: `Inavidata/properties/DiaCmpnt_property_DefaultValue_IDiademAssignmentChannel.htm`*

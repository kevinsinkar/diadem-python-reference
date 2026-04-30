---
title: "IDiademAssignmentChannel.Values"
description: "Specifies the single value of an assignment channel at a specific channel position in the script interface for internal data. You can only read the Values prope"
---

# IDiademAssignmentChannel.Values

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Values for AssignmentChannel <Data>

Specifies the single value of an assignment channel at a specific channel position in the script interface for internal data. You can only read the Values property.

## Signature

```python
obj.Values(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <a href="../idiademassignmentchannel-dvalues/">dValues</a> property to specify and output the numeric values of an assignment channel. The <a href="./">Values</a> property returns the text value of an assignment.</td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn", "Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1", 1)
oMyAssgnList.Add("text2", 2)
oMyAssgnList.Add("text3", 3)
for i in range( 1, 20+1):
    oMyChn.dValues[i] = i
print("Third channel value: " , oMyChn.Values(3))
print("Fourth channel value: " , oMyChn.Values(4))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Values_IDiademAssignmentChannel.htm`*

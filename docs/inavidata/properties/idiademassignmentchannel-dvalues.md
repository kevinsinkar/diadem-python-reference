---
title: "IDiademAssignmentChannel.dValues"
description: "Specifies the single value of an assignment channel at a specific channel position as a Double vector type in the script interface for internal data."
---

# IDiademAssignmentChannel.dValues

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: dValues for AssignmentChannel <Data>

Specifies the single value of an assignment channel at a specific channel position as a Double vector type in the script interface for internal data.

## Signature

```python
obj.dValues(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Use the <span class="Monospace">dvalues</span> property to specify and output the numeric values of an assignment channel. Use the read-only property <span class="Monospace">values</span> to output a text assigned to an assignment channel.</td></tr></table>
</div>

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
for I in range( 1, 20+1):
    oMyChn.dValues[I] = I
dd.MsgBoxDisp("Numeric value: " + oMyChn.dValues(1) + "\r\n" + "Assigned text: " + oMyChn.Values(1))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_dValues_IDiademAssignmentChannel.htm`*

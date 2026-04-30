---
title: "IAssignmentList.FindByValue"
description: "Uses the text to determine an assignment of texts to values in the script interface for internal data."
---

# IAssignmentList.FindByValue

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: FindByValue for AssignmentList <Data>

Uses the text to determine an assignment of texts to values in the script interface for internal data.

## Signature

```python
return_value = obj.FindByValue(Value)
```

## Python example

```python
oMyGrp = dd.Data.Root.ChannelGroups(1)
oMyChn = oMyGrp.Channels.AddAssignmentChannel("MyAssignmentChn","Default Value")
oMyAssgnList = oMyChn.AssignmentList
oMyAssgnList.Add("text1",1)
oMyAssgnList.Add("text2",2)
oMyAssgnList.Add("text3",3)
dd.MsgBoxDisp(oMyAssgnList.FindByValue("text2").Definition)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_FindByValue_IAssignmentList.htm`*

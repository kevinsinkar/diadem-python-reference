---
title: "IDiademAssignmentChannel.Maximum"
description: "Specifies the maximum value of an assignment channel. The value of the Maximum property for Channel corresponds to the value of Object .Properties(\"maximum\").va"
---

# IDiademAssignmentChannel.Maximum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Maximum for AssignmentChannel <Data>

Specifies the maximum value of an assignment channel. The value of the Maximum property for Channel corresponds to the value of Object .Properties("maximum").value .

## Signature

```python
obj.Maximum
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChn = dd.Data.GetChannel("[6]/[4]")
dd.MsgBoxDisp(oMyChn.Maximum) # equivalent to oMyChannel.Properties("maximum").value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Maximum_IDiademAssignmentChannel.htm`*

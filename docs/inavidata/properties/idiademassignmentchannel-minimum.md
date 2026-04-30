---
title: "IDiademAssignmentChannel.Minimum"
description: "Specifies the minimum value of an assignment channel. The value of the Minimum property for AssignmentChannel corresponds to the value of Object .Properties(\"mi"
---

# IDiademAssignmentChannel.Minimum

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: Minimum for AssignmentChannel <Data>

Specifies the minimum value of an assignment channel. The value of the Minimum property for AssignmentChannel corresponds to the value of Object .Properties("minimum").value .

## Signature

```python
obj.Minimum
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChn = dd.Data.GetChannel("[6]/[4]")
dd.MsgBoxDisp(oMyChn.Minimum) # equivalent to oMyChannel.Properties("minimum").value
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_Minimum_IDiademAssignmentChannel.htm`*

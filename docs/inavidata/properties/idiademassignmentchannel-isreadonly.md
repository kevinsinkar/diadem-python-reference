---
title: "IDiademAssignmentChannel.IsReadOnly"
description: "Specifies whether an assignment channel is read-only."
---

# IDiademAssignmentChannel.IsReadOnly

!!! abstract "Property &middot; `Inavidata.chm`"
    Property: IsReadOnly for AssignmentChannel <Data>

Specifies whether an assignment channel is read-only.

## Signature

```python
obj.IsReadOnly
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChn = dd.Data.GetChannel("[6]/[4]")
dd.MsgBoxDisp(oMyChn.IsReadOnly)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/properties/DiaCmpnt_property_IsReadOnly_IDiademAssignmentChannel.htm`*

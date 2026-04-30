---
title: "IDiademAssignmentChannel.RemoveValues"
description: "Deletes the specified values from an assignment channel. DIAdem moves up the subsequent values."
---

# IDiademAssignmentChannel.RemoveValues

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: RemoveValues for AssignmentChannel <Data>

Deletes the specified values from an assignment channel. DIAdem moves up the subsequent values.

## Signature

```python
obj.RemoveValues([Index], [Count])
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChn = dd.Data.Root.ChannelGroups(6).Channels(4)
oMyChn.RemoveValues(3, 4)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_RemoveValues_IDiademAssignmentChannel.htm`*

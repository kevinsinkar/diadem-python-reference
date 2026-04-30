---
title: "IDiademAssignmentChannel.SetValues"
description: "Inserts a numeric value n times at the specified position into an assignment channel."
---

# IDiademAssignmentChannel.SetValues

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: SetValues for AssignmentChannel <Data>

Inserts a numeric value n times at the specified position into an assignment channel.

## Signature

```python
obj.SetValues(newVal, [Index], [Count], [BlockOperationMode])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eValueBlockValueOverwrite` | 0 | DIAdem overwrites existing values (default). |
| `eValueBlockValueInsert` | 1 | DIAdem inserts the values at the specified position. |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "Examples\\Data\\Report_expl.tdm")
oMyChannel = dd.Data.GetChannel("[6]/[4]")
oMyChannel.SetValues(10, 3, 50)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_SetValues_IDiademAssignmentChannel.htm`*

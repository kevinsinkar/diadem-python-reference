---
title: "IDiademAssignmentChannel.SetValuesBlock"
description: "Inserts a block of numeric values from an array into an assignment channel in the Data Portal."
---

# IDiademAssignmentChannel.SetValuesBlock

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: SetValuesBlock for AssignmentChannel <Data>

Inserts a block of numeric values from an array into an assignment channel in the Data Portal.

## Signature

```python
obj.SetValuesBlock(newValArray, [Index], [BlockOperationMode])
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
oMyChn = dd.Data.GetChannel("[6]/[4]")
MyArray = oMyChn.GetValuesBlock(1,2)
oMyChn.SetValuesBlock(MyArray, 3, dd.eValueBlockValueInsert)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_SetValuesBlock_IDiademAssignmentChannel.htm`*

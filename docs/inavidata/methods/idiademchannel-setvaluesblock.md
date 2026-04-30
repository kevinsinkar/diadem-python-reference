---
title: "IDiademChannel.SetValuesBlock"
description: "Inserts a block of values from an array into a channel in the Data Portal."
---

# IDiademChannel.SetValuesBlock

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: SetValuesBlock for Channel <Data>

Inserts a block of values from an array into a channel in the Data Portal.

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
oMyChannel1 = dd.Data.Root.ActiveChannelGroup.Channels(1)
MyArray = oMyChannel1.GetValuesBlock(1,2)
oMyChannel2 = dd.Data.Root.ActiveChannelGroup.Channels(2)
oMyChannel2.SetValuesBlock(MyArray, 1, dd.eValueBlockValueOverwrite)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_SetValuesBlock_IDiademChannel.htm`*

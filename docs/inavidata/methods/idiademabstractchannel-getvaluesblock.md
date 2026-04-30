---
title: "IDiademAbstractChannel.GetValuesBlock"
description: "Reads out a block of values from a channel in the Data Portal and writes these values into an array."
---

# IDiademAbstractChannel.GetValuesBlock

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetValuesBlock for BaseChannel <Data>

Reads out a block of values from a channel in the Data Portal and writes these values into an array.

## Signature

```python
vGetValuesBlock = Object.GetValuesBlock([Index], [Count], [BlockArrayMode])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eValueBlockVbArray` | 0 | VBS Array (Default) |
| `eValueBlockSafeArray` | 1 | Type-safe array. You cannot access this array from VBS scripts. However, you can exchange the data with other applications that expect type-safe arrays. |
| `eValueBlockDValueVbArray` | 2 | VBS array with double values |
| `eValueBlockDValueSafeArray` | 3 | Type-safe array with double values. You cannot access this array from VBS scripts. However, you can exchange the data with other applications that expect type-safe arrays. |

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

*Source: `Inavidata/methods/DiaCmpnt_method_GetValuesBlock_IDiademAbstractChannel.htm`*

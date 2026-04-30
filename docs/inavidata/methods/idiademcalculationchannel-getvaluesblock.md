---
title: "IDiademCalculationChannel.GetValuesBlock"
description: "Reads a block of values from a calculation channel in the Data Portal and writes these values into an array."
---

# IDiademCalculationChannel.GetValuesBlock

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetValuesBlock for CalculationChannel <Data>

Reads a block of values from a calculation channel in the Data Portal and writes these values into an array.

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
oMyCalculationChn = dd.Data.Root.ChannelGroups(1).Channels.AddCalculationChannel("Result", "=Speed * 2", "m/s", 1)
oMyCalculationChn.RunCalculation()
MyArray = oMyCalculationChn.GetValuesBlock(1,2)
for I in range( 0, len(MyArray)-1):
    print (MyArray(I))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_GetValuesBlock_IDiademCalculationChannel.htm`*

---
title: "IDiademImplicitChannel.GetValuesBlock"
description: "Reads out a block of values from an implicit channel in the Data Portal and writes these values into an array."
---

# IDiademImplicitChannel.GetValuesBlock

!!! abstract "Method &middot; `Inavidata.chm`"
    Method: GetValuesBlock for ImplicitChannel <Data>

Reads out a block of values from an implicit channel in the Data Portal and writes these values into an array.

## Signature

```python
vGetValuesBlock = Object.GetValuesBlock([Index], [Count], [BlockArrayMode])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If the sum of the parameters <span class="Monospace">Index</span> and <span class="Monospace">Count</span> is greater than the value of <span class="Monospace">Channel.Size</span>,  DIAdem outputs an error.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>If the channel to be read out is a date/time channel, the values of the result array are a <span class="Monospace">vbDate</span> type.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eValueBlockVbArray` | 0 | VBS Array (Default) |
| `eValueBlockSafeArray` | 1 | Type-safe array. You cannot access this array from VBS scripts. However, you can exchange the data with other applications that expect type-safe arrays. |
| `eValueBlockDValueVbArray` | 2 | VBS array with double values |
| `eValueBlockDValueSafeArray` | 3 | Type-safe array with double values. You cannot access this array from VBS scripts. However, you can exchange the data with other applications that expect type-safe arrays. |

## Python example

```python
dd.Data.Root.Clear()
oMyGroup = dd.Data.Root.ChannelGroups.Add("MyGroup")
oMyImplChannel = dd.Data.Root.ActiveChannelGroup.Channels.AddImplicitChannel("MyImplChn", 1, 1, 100,dd.DataTypeFloat64)
MyArray = oMyImplChannel.GetValuesBlock(1,2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Concatenate Channels</a> | <a href="#" data-unresolved="1">Sorting Channel Groups</a> | <a href="#" data-unresolved="1">Sorting the Channels in the Default-Group</a></p>
</div>
</div>

---

*Source: `Inavidata/methods/DiaCmpnt_method_GetValuesBlock_IDiademImplicitChannel.htm`*

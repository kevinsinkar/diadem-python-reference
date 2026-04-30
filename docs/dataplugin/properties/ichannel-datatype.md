---
title: "IChannel.DataType"
description: "Returns the data type of a channel."
---

# IChannel.DataType

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: DataType for Channel <DataPlugin>

Returns the data type of a channel.

## Signature

```python
obj.DataType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eNoType` | 0 | Not defined |
| `eI8` | 1 | 8-bit integer values |
| `eI16` | 2 | 16-bit integer values |
| `eI32` | 3 | 32-bit integer values |
| `eI64` | 4 | 64-bit integer values |
| `eByte` | 5 | Byte |
| `eU16` | 6 | 16-bit unsigned integer |
| `eU32` | 7 | 32-bit unsigned integer |
| `eU64` | 8 | 64-bit unsigned integer |
| `eR32` | 9 | 32-bit real values |
| `eR64` | 10 | 64-bit real values |
| `eString` | 23 | Text |
| `eEnum` | 24 | Enumeration |
| `eTime` | 30 | Time values |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in Root.ChannelGroups(1).Channels:
    if (oMyChn.IsKindOf(eNormal)):
        oMyChn.Properties.Add("DataType", oMyChn.DataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Examples</h2><p class="body"><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_DataType_IChannel.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

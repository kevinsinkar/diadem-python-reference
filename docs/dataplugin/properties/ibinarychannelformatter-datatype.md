---
title: "IBinaryChannelFormatter.Datatype"
description: "Specifies the data type of a DirectAccess channel that is associated with a BinaryBlock."
---

# IBinaryChannelFormatter.Datatype

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: DataType for BinaryChannelFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the data type of a DirectAccess channel that is associated with a BinaryBlock.

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
for oMyChn in oBlock.Channels:
    if oMyChn.Formatter.IsKindOf(eStringBlock):
        oMyChn.Properties.Add("StringBlock", oMyChn.Formatter.DataType)
    elif oMyChn.Formatter.IsKindOf(eBinaryBlock):
        oMyChn.Properties.Add("BinaryBlock", oMyChn.Formatter.DataType)
    elif oMyChn.Formatter.IsKindOf(eFixedWidthBlock):
        oMyChn.Properties.Add("FixedWidthBlock", oMyChn.Formatter.DataType)
    elif oMyChn.Formatter.IsKindOf(eCellBlock):
        oMyChn.Properties.Add("CellBlock", oMyChn.Formatter.DataType)
```

## See also

<div markdown="1">
<div class="SeeAlso">
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_Property_Datatype_IBinaryChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IBinaryChannelFormatter.ByteOrder"
description: "Specifies the byte order for a channel in the file if the data type consists of several bytes."
---

# IBinaryChannelFormatter.ByteOrder

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: ByteOrder for BinaryChannelFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Specifies the byte order for a channel in the file if the data type consists of several bytes.

## Signature

```python
obj.ByteOrder
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLittleEndian` | 1 | The first byte is the higher-value byte. |
| `eBigEndian` | 2 | The last byte is the higher-value byte. |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oChn.Factor = 5
oChn.Offset = 50
oChn.Formatter.ByteOrder = eBigEndian
oMyGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso">
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_Property_ByteOrder_IBinaryChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

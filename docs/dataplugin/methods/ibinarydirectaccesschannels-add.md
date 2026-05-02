---
title: "IBinaryDirectAccessChannels.Add"
description: "Adds an object to the Channels collection of a BinaryBlock and returns a DirectAccessChannel object."
---

# IBinaryDirectAccessChannels.Add

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: Add for BinaryDirectAccessChannels

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Adds an object to the Channels collection of a BinaryBlock and returns a DirectAccessChannel object.

## Signature

```python
return_value = obj.Add(Name, DataType, [ContiguousValues])
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eNoType` | 0 | Not defined |
| `eI8` | 1 | 8-bit integer |
| `eByte` | 5 | Byte |
| `eI16` | 2 | 16-bit integer |
| `eI32` | 3 | 32-bit integer |
| `eI64` | 4 | 64-bit integer |
| `eR32` | 9 | 32-bit real |
| `eR64` | 10 | 64-bit real |
| `eTime` | 30 | Time |
| `eString` | 23 | Text |
| `eU64` | 8 | 64-bit unsigned integer |
| `eU32` | 7 | 32-bit unsigned integer |
| `eU16` | 6 | 16-bit unsigned integer |
| `eEnum` | 24 | Enumeration |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python

```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_Add_IBinaryDirectAccessChannels.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

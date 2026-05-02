---
title: "IStringChannelFormatter.IsKindOf"
description: "Checks whether a StringChannelFormatter object is a certain type."
---

# IStringChannelFormatter.IsKindOf

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: IsKindOf for StringChannelFormatter

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Checks whether a StringChannelFormatter object is a certain type.

## Signature

```python
bIsKindOf = Object.IsKindOf(Type)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBinaryBlock` | 0 | BinaryBlock type block |
| `eStringBlock` | 1 | StringBlock type block |
| `eFixedWidthBlock` | 2 | FixedWidthBlock type block |
| `eCellBlock` | 3 | CellBlock type block |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
for oMyChn in oBlock.Channels:
    if (oMyChn.Formatter.IsKindOf(eStringBlock)):
        oMyChn.Properties.Add("DataType", oMyChn.Formatter.DataType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_IsKindOf_IStringChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

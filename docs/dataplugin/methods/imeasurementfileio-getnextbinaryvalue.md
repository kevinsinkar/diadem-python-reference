---
title: "IMeasurementFileIO.GetNextBinaryValue"
description: "Reads a value at the current file position and moves the file pointer according to the data type of the value."
---

# IMeasurementFileIO.GetNextBinaryValue

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetNextBinaryValue for File

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Reads a value at the current file position and moves the file pointer according to the data type of the value.

## Signature

```python
vGetNextBinaryValue = Object.GetNextBinaryValue(DataType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>If you specify the data types eU16 or eU32, the return value <em>Value</em> can cause problems in VBS.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eI8` | 1 | 8-bit integer values |
| `eI16` | 2 | 16-bit integer values |
| `eI32` | 3 | 32-bit integer values |
| `eI64` | 4 | 64-bit integer values |
| `eByte` | 5 | Byte |
| `eU16` | 6 | 16-bit unsigned integer |
| `eU32` | 7 | 32-bit unsigned integer |
| `eR32` | 9 | 32-bit real values |
| `eR64` | 10 | 64-bit real values |

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
MyAttr = File.GetNextBinaryValue(eI32)
Root.Properties.Add("Attr1", MyAttr)
MyAttr = File.GetNextBinaryValue(eU32)
Root.Properties.Add("Attr2", MyAttr)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetNextBinaryValue_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

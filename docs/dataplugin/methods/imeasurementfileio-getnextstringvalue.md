---
title: "IMeasurementFileIO.GetNextStringValue"
description: "Reads a value at the current file position and moves the file pointer according to the data type of the value."
---

# IMeasurementFileIO.GetNextStringValue

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetNextStringValue for File

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
vGetNextStringValue = Object.GetNextStringValue(DataType)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note</strong>  Because <span class="Monospace">GetNextStringValue</span> does not advance past the end of the line, you must use File.<a href="../imeasurementfileio-skipline/">SkipLine</a> to position the file pointer in the next line.</td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
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
File.Formatter.LineFeeds = "\n"
File.Formatter.Delimiters = ":"
while not File.Position == File.Size:
    PropName  = File.GetNextStringValue(eString)
    PropValue = File.GetNextStringValue(eString)
    Root.Properties.Add(PropName, PropValue)
    File.SkipLine()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetNextStringValue_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

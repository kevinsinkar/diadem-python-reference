---
title: "IMeasurementFileIO.GetLineFeed"
description: "Determines the line end character in the file."
---

# IMeasurementFileIO.GetLineFeed

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetLineFeed for File

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Determines the line end character in the file.

## Signature

```python
sGetLineFeed = Object.GetLineFeed(StartPosition, NrOfBytes)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
28.06.2004 16:28:20; 0,001234¶
28.06.2004 16:28:21; 0,002398¶
28.06.2004 16:28:22; 0,001296¶
28.06.2004 16:28:23; 0,001628¶
28.06.2004 16:28:24; 0,001683¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = File.GetLineFeed()
File.Formatter.TimeFormat = "DD.MM.YYYY hh:mm:ss"
File.Formatter.Delimiters = ";"
File.Formatter.DecimalPoint = ","
while File.Position != File.Size:
    ValueTime = File.GetNextStringValue(eTime)
    Value = File.GetNextStringValue(eR64)
    Fill.SkipLine()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetLineFeed_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

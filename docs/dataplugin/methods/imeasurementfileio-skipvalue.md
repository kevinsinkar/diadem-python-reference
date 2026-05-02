---
title: "IMeasurementFileIO.SkipValue"
description: "Skips a value in a line."
---

# IMeasurementFileIO.SkipValue

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: SkipValue for File

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Skips a value in a line.

## Signature

```python
bSkipValue = Object.SkipValue
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
XAxis; ;1.000.000; 2.000; 301¶
```

```python
File.Formatter.LineFeeds = "\n"
File.Formatter.Delimiters = ";"
File.Formatter.ThousandSeparator = "."
File.SkipValue()
oMyGrp.Channels.AddImplicitChannel(ChannelName, StartValue, Increment, ChannelSize, eI32)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_SkipValue_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

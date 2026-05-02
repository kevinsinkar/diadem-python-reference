---
title: "IMeasurementFileIO.SkipValues"
description: "Skips several values in a line."
---

# IMeasurementFileIO.SkipValues

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: SkipValues for File

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Skips several values in a line.

## Signature

```python
iSkipValues = Object.SkipValues(Number)
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
ChannelName = File.GetNextStringValue(eString)
File.SkipValues(3)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_SkipValues_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

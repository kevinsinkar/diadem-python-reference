---
title: "IMeasurementFileIO.GetFixedWidthBlock"
description: "Reads a text file and returns the channel values contained in the file."
---

# IMeasurementFileIO.GetFixedWidthBlock

!!! abstract "Method &middot; `DataPlugin.chm`"
    Method: GetFixedWidthBlock for File

!!! note "Context: DataPlugin script"
    Examples in this section run inside DIAdem's **DataPlugin host**
    context, where identifiers like `Root`, `File`, `oBlock`, and
    related host-supplied objects resolve automatically. From standalone
    external Python via `Dispatch("DIAdem.TOCmd")` those names raise
    `NameError`. The DataPlugin API is intended to be used by writing
    your script inside a `.uri` DataPlugin file that DIAdem then loads;
    it is not directly callable from external Python.

Reads a text file and returns the channel values contained in the file.

## Signature

```python
return_value = obj.GetFixedWidthBlock
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img border="0" height="25" src="../Image/NOTE.GIF" width="26"/></td><td><strong>Note  </strong>The file pointer of the binary file does not move when a BinaryBlock is read.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
oChn1.Formatter.CharacterCount = 4
oChn1.Formatter.SampleWidth = 2
oChannelGroup.Channels.AddDirectAccessChannel(oChn1)
oBlock.Position = File.Position
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Methods/DataPlugin_method_GetFixedWidthBlock_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

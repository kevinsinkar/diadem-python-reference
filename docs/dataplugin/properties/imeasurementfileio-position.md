---
title: "IMeasurementFileIO.Position"
description: "Specifies the current position of the file pointer."
---

# IMeasurementFileIO.Position

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Position for File

Specifies the current position of the file pointer.

## Signature

```python
obj.Position
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
File.Formatter.LineFeeds = vbNewLine
File.Formatter.Delimiters = ":"
while File.Position != File.Size:
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

*Source: `DataPlugin/Properties/DataPlugin_property_Position_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

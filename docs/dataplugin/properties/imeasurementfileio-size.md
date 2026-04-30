---
title: "IMeasurementFileIO.Size"
description: "Returns the current size of the file in bytes."
---

# IMeasurementFileIO.Size

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Size for File

Returns the current size of the file in bytes.

## Signature

```python
obj.Size
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
File.Formatter.LineFeeds = vbNewLine
File.Formatter.Delimiters = ":"
while not File.Position = File.Size:
    PropName  = File.GetNextStringValue(eString)
    PropValue = File.GetNextStringValue(eString)
    Root.Properties.Add(PropName, PropValue)
    File.SkipLine()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Size_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IMeasurementFileIO.Formatter"
description: "Returns the Formatter object that contains information about the format of the file that the DataPlugin is currently processing."
---

# IMeasurementFileIO.Formatter

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: Formatter for File

Returns the Formatter object that contains information about the format of the file that the DataPlugin is currently processing.

## Signature

```python
return_value = obj.Formatter
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

File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.TimeFormat = "DD.MM.YYYY hh:mm:ss"
File.Formatter.Delimiters = ";"
File.Formatter.DecimalPoint = ","
while (File.Position != File.Size):
    ValueTime = File.GetNextStringValue(eTime)
    Value = File.GetNextStringValue(eR64)
    File.SkipLine()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Object overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_Formatter_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

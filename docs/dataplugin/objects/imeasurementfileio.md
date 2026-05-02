---
title: "IMeasurementFileIO"
description: "The File object provides information such as the name, origin, and size of the file the DataPlugin is currently processing. You use the File object properties t"
---

# IMeasurementFileIO

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: File

The File object provides information such as the name, origin, and size of the file the DataPlugin is currently processing. You use the File object properties to specify the special format of this file. The file is either a text file or a binary file. Use the methods of the File object to access this file. You can use the methods to read single values, texts, or sections from the file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
File.Formatter.LineFeeds = "\n"
File.Formatter.Delimiters = ":"
while (File.Position != File.Size):
    PropName  = File.GetNextStringValue(eString)
    PropValue = File.GetNextStringValue(eString)
    Root.Properties.Add(PropName, PropValue)
    File.SkipLine()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/imeasurementfileio-formatter/">Formatter</a> | <a href="../../properties/imeasurementfileio-info/">Info</a> | <a href="../../properties/imeasurementfileio-position/">Position</a> | <a href="../../properties/imeasurementfileio-size/">Size</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/imeasurementfileio-getbinaryblock/">GetBinaryBlock</a> | <a href="../../methods/imeasurementfileio-getcharacters/">GetCharacters</a> | <a href="../../methods/imeasurementfileio-getfixedwidthblock/">GetFixedWidthBlock</a> | <a href="../../methods/imeasurementfileio-getlinefeed/">GetLineFeed</a> | <a href="../../methods/imeasurementfileio-getnextbinaryvalue/">GetNextBinaryValue</a> | <a href="../../methods/imeasurementfileio-getnextline/">GetNextLine</a> | <a href="../../methods/imeasurementfileio-getnextstringvalue/">GetNextStringValue</a> | <a href="../../methods/imeasurementfileio-getstringblock/">GetStringBlock</a> | <a href="../../methods/imeasurementfileio-skipline/">SkipLine</a> | <a href="../../methods/imeasurementfileio-skiplines/">SkipLines</a> | <a href="../../methods/imeasurementfileio-skipvalue/">SkipValue</a> | <a href="../../methods/imeasurementfileio-skipvalues/">SkipValues</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../idataplugin/">DataPlugin</a>.<a href="../../methods/idataplugin-openfile/">OpenFile</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IMeasurementFileIO.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

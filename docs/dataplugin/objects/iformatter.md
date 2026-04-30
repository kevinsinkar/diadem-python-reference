---
title: "IFormatter"
description: "The Formatter object contains information about the format of the file that the DataPlugin is currently processing."
---

# IFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: Formatter

The Formatter object contains information about the format of the file that the DataPlugin is currently processing.

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
File.Formatter.LineFeeds  = vbNewLine
File.Formatter.TimeFormat = "DD.MM.YYYY hh:mm:ss"
File.Formatter.Delimiters = ";"
File.Formatter.DecimalPoint = ","
while (File.Position != File.Size):
    ValueTime = File.GetNextStringValue(eTime)
    Value = File.GetNextStringValue(eR64)
    File.SkipLine()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/iformatter-byteorder/">ByteOrder</a> | <a href="../../properties/iformatter-characterformat/">CharacterFormat</a> | <a href="../../properties/iformatter-commentsign/">CommentSign</a> | <a href="../../properties/iformatter-decimalpoint/">DecimalPoint</a> | <a href="../../properties/iformatter-delimiters/">Delimiters</a> | <a href="../../properties/iformatter-exponentseparator/">ExponentSeparator</a> | <a href="../../properties/iformatter-ignoreemptylines/">IgnoreEmptyLines</a> | <a href="../../properties/iformatter-linefeeds/">LineFeeds</a> | <a href="../../properties/iformatter-novaluesign/">NoValueSign</a> | <a href="../../properties/iformatter-stringsign/">StringSign</a> | <a href="../../properties/iformatter-thousandseparator/">ThousandSeparator</a> | <a href="../../properties/iformatter-timeformat/">TimeFormat</a> | <a href="../../properties/iformatter-trimcharacters/">TrimCharacters</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/iformatter-parsestring/">ParseString</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

---
title: "IFormatter.StringSign"
description: "Specifies the character that identifies the beginning and the end of a text. The text identifier is ignored when the text is read. Text between two text identif"
---

# IFormatter.StringSign

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: StringSign for Formatter

Specifies the character that identifies the beginning and the end of a text. The text identifier is ignored when the text is read. Text between two text identifiers are not interpreted when text is read.

## Signature

```python
obj.StringSign
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
"Cloudy";   18.8¶
"Overcast"; 22.5¶
"Sunny";    25.3¶
"Cloudy";   21.2¶
"Rain";     18.0¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.Delimiters = ";"
File.Formatter.StringSign = Char(34)

oGrp.Channels.AddDirectAccessChannel(oChn1)
oGrp.Channels.AddDirectAccessChannel(oChn2)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_StringSign_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

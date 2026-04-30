---
title: "IStringChannelFormatter.TimeFormat"
description: "Specifies the format for the channel time values in the file."
---

# IStringChannelFormatter.TimeFormat

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: TimeFormat for StringChannelFormatter

Specifies the format for the channel time values in the file.

## Signature

```python
obj.TimeFormat
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>The year formatting automatically extends to 4 characters so that the specification YY becomes YYYY. When DIAdem reads in the data, the correct century precedes. The year 99 becomes 1999 and the year 05 becomes 2005. </td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="../image/note.gif" width="26"/></td><td><strong>Note  </strong>Normally seconds and minutes are in the value range 0-59, hours in the value range 0-23, days in the value range 1-31, and months in the values range 1-12. If one of these values to be read exceeds its value range, the value is converted into the next value. For example, the time value 00:65:10 in the file becomes 01:05:10 and the time value 54:30:00 becomes 03.01.0000 06:10:00.</td></tr></table>
</div>

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
28.06.2004 16:28:20;  28/06/2011 16-28-20¶
28.06.2004 16:28:21;  28/06/2011 16-28-21¶
28.06.2004 16:28:22;  28/06/2011 16-28-22¶
28.06.2004 16:28:23;  28/06/2011 16-28-23¶
28.06.2004 16:28:24;  28/06/2011 16-28-24¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = vbNewLine
File.Formatter.Delimiters = ";"
File.Formatter.TimeFormat = "DD.MM.YYYY hh:mm:ss"

oBlock = File.GetStringBlock()
oGrp = Root.ChannelGroups.Add("MyChannelGroup")
oChn = oBlock.Channels.Add("Date1",eTime)
oGrp.Channels.AddDirectAccessChannel(oChn)
oChn = oBlock.Channels.Add("Date2",eTime)
oChn.Formatter.TimeFormat = "DD/MM/YYYY hh-mm-ss"
oGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_TimeFormat_IStringChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

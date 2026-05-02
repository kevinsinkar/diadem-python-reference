---
title: "IFormatter.TimeFormat"
description: "Specifies the format for the time values in the file."
---

# IFormatter.TimeFormat

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: TimeFormat for Formatter

Specifies the format for the time values in the file.

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
28.06.2004 16:28:20; 0.001234¶
28.06.2004 16:28:21; 0.002398¶
28.06.2004 16:28:22; 0.001296¶
28.06.2004 16:28:23; 0.001628¶
28.06.2004 16:28:24; 0.001683¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.Delimiters = ";"
File.Formatter.TimeFormat = "DD.MM.YYYY hh:mm:ss"
oGrp = Root.ChannelGroups.Add("MyChannelGroup")
oChn = oBlock.Channels.Add("Time",eTime)
oGrp.Channels.AddDirectAccessChannel(oChn)
oChn = oBlock.Channels.Add("YShift",eR64)
oGrp.Channels.AddDirectAccessChannel(oChn)
```

```python
54:30:0¶
60:30:0¶
66:30:0¶
72:30:0¶
78:30:0¶
84:30:0¶
90:30:0¶
```

```python
File.Formatter.Delimiters = ";"
File.Formatter.LineFeeds  = "\n"
File.Formatter.TimeFormat = "hh:mm:ss"


oGrp.Channels.AddDirectAccessChannel(oDAChn)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_TimeFormat_IFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

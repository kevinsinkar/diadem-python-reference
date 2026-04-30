---
title: "IStringChannelFormatter.ThousandSeparator"
description: "Specifies the thousands separator, which is ignored when channel values are read in."
---

# IStringChannelFormatter.ThousandSeparator

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: ThousandSeparator for StringChannelFormatter

Specifies the thousands separator, which is ignored when channel values are read in.

## Signature

```python
obj.ThousandSeparator
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
1.000.000; 1,000¶
2.000.000; 2,000¶
3.000.000; 3,000¶
4.000.000; 4,000¶
5.000.000; 5,000¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = vbNewLine
File.Formatter.Delimiters = ";"
File.Formatter.ThousandSeparator = "."

oBlock = File.GetStringBlock()
oGrp = Root.ChannelGroups.Add("MyChannelGroup")
oChn = oBlock.Channels.Add("Date1",eTime)
oGrp.Channels.AddDirectAccessChannel(oChn)
oChn = oBlock.Channels.Add("Date2",eTime)
oChn.Formatter.NoValueSign = "$$$"
oGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_ThousandSeparator_IStringChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

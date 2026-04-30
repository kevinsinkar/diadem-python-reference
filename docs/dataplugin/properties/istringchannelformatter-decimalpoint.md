---
title: "IStringChannelFormatter.DecimalPoint"
description: "Specifies the decimal symbol used in a channel."
---

# IStringChannelFormatter.DecimalPoint

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: DecimalPoint for StringChannelFormatter

Specifies the decimal symbol used in a channel.

## Signature

```python
obj.DecimalPoint
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
0,001234; 1.941434¶
0,002398; 2.342393¶
0,001296; 3.451496¶
0,001628; 4.071624¶
0,001683; 5.261483¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = vbNewLine
File.Formatter.DecimalPoint = ","
File.Formatter.Delimiters = ";"

oBlock = File.GetStringBlock()
oGrp = Root.ChannelGroups.Add("MyChannelGroup")
oChn = oBlock.Channels.Add("Date1",eTime)
oGrp.Channels.AddDirectAccessChannel(oChn)
oChn = oBlock.Channels.Add("Date2",eTime)
oChn.Formatter.DecimalPoint = "."
oGrp.Channels.AddDirectAccessChannel(oChn)
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>Procedures</h2><h2>Examples</h2><p><a href="#" data-unresolved="1">Checking DataPlugins for Timeout</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_property_DecimalPoint_IStringChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

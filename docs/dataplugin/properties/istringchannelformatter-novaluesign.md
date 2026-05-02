---
title: "IStringChannelFormatter.NoValueSign"
description: "Specifies the NoValue character used in a channel."
---

# IStringChannelFormatter.NoValueSign

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: NoValueSign for StringChannelFormatter

Specifies the NoValue character used in a channel.

## Signature

```python
obj.NoValueSign
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
0,001234; 1,941434¶
0,002398; $$$¶
NV; 3,451496¶
0,001628; $$$¶
0,001683; 5,261483¶
```

```python
File.Formatter.TrimCharacters = " "
File.Formatter.LineFeeds  = "\n"
File.Formatter.DecimalPoint = ","
File.Formatter.Delimiters = ";"
File.Formatter.NoValueSign = "NV"

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

*Source: `DataPlugin/Properties/DataPlugin_property_NoValueSign_IStringChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

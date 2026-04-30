---
title: "IFixedWidthChannelFormatter"
description: "The FixedWidthChannelFormatter object contains information about how the values of a channel are represented in the text file."
---

# IFixedWidthChannelFormatter

!!! abstract "Object &middot; `DataPlugin.chm`"
    Object: FixedWidthChannelFormatter

The FixedWidthChannelFormatter object contains information about how the values of a channel are represented in the text file.

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
0127+098
0000-876
-128+654
```

```python
oChn1.Formatter.CharacterCount = 4
oChn1.Formatter.SampleWidth = 1
oChannelGroup.Channels.AddDirectAccessChannel(oChn1)

oChn2.Formatter.CharacterCount = 4
oChn2.Formatter.SampleWidth = 1

oChannelGroup.Channels.AddDirectAccessChannel(oChn2)
oBlock.Position = File.Position
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p class="Body"><a href="../../properties/ifixedwidthchannelformatter-block/">Block</a> | <a href="../../properties/ifixedwidthchannelformatter-charactercount/">CharacterCount</a> | <a href="../../properties/ifixedwidthchannelformatter-datatype/">DataType</a> | <a href="../../properties/ifixedwidthchannelformatter-samplewidth/">SampleWidth</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p class="Body"><a href="../../methods/iabstractchannelformatter-iskindof/">IsKindOf</a></p></div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Objects/DataPlugin_Objects_IFixedWidthChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

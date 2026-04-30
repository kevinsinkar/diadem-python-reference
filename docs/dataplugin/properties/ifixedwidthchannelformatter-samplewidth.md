---
title: "IFixedWidthChannelFormatter.SampleWidth"
description: "Specifies how many consecutive values are read from a line in the text file for one channel. The default value for this property is 1."
---

# IFixedWidthChannelFormatter.SampleWidth

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: SampleWidth for FixedWidthChannelFormatter

Specifies how many consecutive values are read from a line in the text file for one channel. The default value for this property is 1.

## Signature

```python
obj.SampleWidth
```

## Python example

!!! warning "Machine-translated"
    The original DIAdem topic did not include a Python tab; this
    example was machine-translated from the VBScript source.

```python
0127+098-765+432
0000-876+543+210
-128+654-321
```

```python
oChn1.Formatter.CharacterCount = 4
oChn1.Formatter.SampleWidth = 2
oChannelGroup.Channels.AddDirectAccessChannel(oChn1)

oChn2.Formatter.CharacterCount = 4
oChn2.Formatter.SampleWidth = 2
oChannelGroup.Channels.AddDirectAccessChannel(oChn2)

oBlock.Position = File.Position
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `DataPlugin/Properties/DataPlugin_Property_SampleWidth_IFixedWidthChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

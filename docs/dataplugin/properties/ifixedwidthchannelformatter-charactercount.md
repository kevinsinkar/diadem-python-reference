---
title: "IFixedWidthChannelFormatter.CharacterCount"
description: "Specifies the number of characters that are read from the text file per channel value. The default value for this property is 10."
---

# IFixedWidthChannelFormatter.CharacterCount

!!! abstract "Property &middot; `DataPlugin.chm`"
    Property: CharacterCount for FixedWidthChannelFormatter

Specifies the number of characters that are read from the text file per channel value. The default value for this property is 10.

## Signature

```python
obj.CharacterCount
```

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

*Source: `DataPlugin/Properties/DataPlugin_Property_CharacterCount_IFixedWidthChannelFormatter.htm`&nbsp;&middot;&nbsp;Python translated from VBS*

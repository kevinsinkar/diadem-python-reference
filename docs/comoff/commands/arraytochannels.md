---
title: "ArrayToChannels"
description: "Converts an array into channels."
---

# ArrayToChannels

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ArrayToChannels

Converts an array into channels.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  You must return the channel names as an array.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem tries to automatically specify the data type of new channels from the values of the array to be converted.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">SrcVariant</td>
<td>Specifies the name of the variant that DIAdem converts into channels.<div id="exp_SrcVariant">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChannelNames</td>
<td>Specifies the names of the channels.<div id="exp_ChannelNames">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[OverWriteMode]</td>
<td>Specifies whether DIAdem overwrites the values or appends the values. The default value is <span class="Monospace">FALSE</span>, which means that DIAdem appends the values.<div id="exp_OverWriteMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[TransposeMatrix]</td>
<td>Specifies whether DIAdem transposes the matrix, which means DIAdem exchanges the rows and columns. The default value is <span class="Monospace">FALSE</span> which means that DIAdem does not swap the rows and columns.<div id="exp_TransposeMatrix">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies a channel list as a vector in the script environment. The return value is a ChannelList type.<div id="exp_ChannelList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
PI = math.pi
ChannelLength=10000
NoOfChannels = 2
#The 2D array is preset with 0 here.
MyArray = [[0 for x in range(ChannelLength+1)] for y in range(NoOfChannels)]
for I in range(0, 10000 + 1):
    MyArray[0][I] = (2.0 * PI *float(I)) / float(ChannelLength)
    MyArray[1][I] = math.sin((2.0*PI*I) / ChannelLength )
MyChannels=["Result/XChannel","Result/SinChannel"]
dd.ArrayToChannels(MyArray, MyChannels)
```

---

*Source: `ComOff/ArrayToChannels.htm`*

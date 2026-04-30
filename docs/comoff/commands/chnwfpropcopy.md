---
title: "ChnWfPropCopy"
description: "Copies the waveform properties of a waveform channel to another channel. The channel whose waveform properties you want to copy must be a waveform channel. When"
---

# ChnWfPropCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnWfPropCopy

Copies the waveform properties of a waveform channel to another channel. The channel whose waveform properties you want to copy must be a waveform channel. When you convert an xy-channel to a waveform channel, DIAdem automatically removes the xy relationship.

## Signature

```python
dd.ChnWfPropCopy( Y , Y1 )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel to which you want copy the waveform properties. If the channel is not a waveform channel, DIAdem converts this channel into a waveform channel.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the waveform channel with the waveform properties you want to copy. If the channel from which the waveform properties are to be copied is not a waveform, DIAdem outputs an error message. You can prevent the error message if you use the <a href="../../../inavidata/methods/idiademabstractchannel-iskindof/">IsKindOf</a> method to check whether the source channel is a waveform channel before you call the command.</td></tr>
</table>
</div>

## Python example

```python
if (dd.Data.Root.ChannelGroups(1).Channels("WfChn").IsKindOf(dd.eDataChannelWF)) :
    dd.ChnWfPropCopy(dd.Data.Root.ChannelGroups(1).Channels("Chn"), dd.Data.Root.ChannelGroups(1).Channels("WfChn"))
else:
    print("Source channel is not a waveform channel.")
```

---

*Source: `ComOff/ChnWfPropCopy.htm`*

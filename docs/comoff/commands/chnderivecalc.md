---
title: "ChnDeriveCalc"
description: "Differentiates a signal numerically by calculating the central difference quotient of the second order."
---

# ChnDeriveCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDeriveCalc

Differentiates a signal numerically by calculating the central difference quotient of the second order.

## Signature

```python
return_value = dd.ChnDeriveCalc( XW , Y , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. If the y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyResultChn = dd.ChnDeriveCalc(oMyXChannel, oMyYChannel, "Results/Derivation")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

```python
oMyResultChn = dd.ChnDeriveCalc("[1]/[1]", "[1]/[2]", "Results/Derivation")
print("Result channel: " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnDeriveCalc.htm`*

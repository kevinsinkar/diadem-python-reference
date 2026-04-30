---
title: "ChnDurationCalc"
description: "Calculates the time at level. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific lower thres"
---

# ChnDurationCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDurationCalc

Calculates the time at level. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific lower threshold.

## Signature

```python
return_value = dd.ChnDurationCalc( XW , Y , CalcInjury, X1 , Y1 , ResultChannel , ResultChannel , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">Time at Level</a> for more information on the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel with time values of the signal. If all other channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal.</td></tr>
<tr><td width="150">CalcInjury</td>
<td>Specifies whether DIAdem calculates the limit curve for the time-at-level.<div id="exp_CalcInjury">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel containing the time values of the limit in seconds.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the amplitude values of the limits.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the load duration.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the injury values.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains three result channels. The first result channel contains the load duration, the second result channel contains the amplitudes, and the third result channel contains the injury values. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyX1Channel = dd.Data.Root.ChannelGroups(1).Channels(3)
oMyY1Channel = dd.Data.Root.ChannelGroups(1).Channels(4)
oMyResultChn = dd.ChnDurationCalc(oMyXChannel, oMyYChannel, True, oMyX1Channel, oMyY1Channel, "Results/LoadDuration", "Results/Amplitude", "Results/Injury")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name)
```

```python
oMyResultChn = dd.ChnDurationCalc("[1]/[1]","[1]/[2]", True, "[1]/[3]","[1]/[4]","Results/LoadDuration", "Results/Amplitude", "Results/Injury")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name)
```

---

*Source: `ComOff/ChnDurationCalc.htm`*

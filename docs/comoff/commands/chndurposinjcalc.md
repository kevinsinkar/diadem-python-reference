---
title: "ChnDurPosInjCalc"
description: "Calculates the time-at-level and the injury risk for positive limit curves. The time at level describes the maximum continuous time interval in which the amplit"
---

# ChnDurPosInjCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDurPosInjCalc

Calculates the time-at-level and the injury risk for positive limit curves. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific threshold.

## Signature

```python
return_value = dd.ChnDurPosInjCalc( X , Y , X1 , Y1 , DurationType, ResultChannel , ResultChannel , ResultChannel , CalcSteps, CalcDuration)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">Time at Level</a> for more information on the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel with time values of the signal in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel containing the time values of the positive boundary curve, in seconds.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the amplitude values of the positive limit curve.</td></tr>
<tr><td width="150">DurationType</td>
<td>Specifies whether DIAdem calculates the time-at-level from one section or several sections.<div id="exp_DurationType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"in one peak"</pre></donottranslate></td>
<td>In one peak</td></tr>
<tr><td width="150"><donottranslate><pre>"in multiple peaks"</pre></donottranslate></td>
<td>In multiple peaks</td></tr>
<tr><td width="150"><donottranslate><pre>"in one peak (custom)"</pre></donottranslate></td>
<td>In one peak (adjusted)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the load durations.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the injury probability.</td></tr>
<tr><td width="150">CalcSteps</td>
<td>Specifies the number of steps for the user-defined time-at-level calculation.<div id="exp_CalcSteps">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>2 &lt;= CalcSteps &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CalcDuration</td>
<td>Specifies the duration of the user-defined time-at-level calculation.<div id="exp_CalcDuration">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>1 &lt;= CalcDuration &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains three result channels. The first result channel contains the load duration, the second result channel contains the amplitudes, and the third result channel contains the injury probability. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(2).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(2).Channels(2)
oMyX1Channel = dd.Data.Root.ChannelGroups(2).Channels(3)
oMyY1Channel = dd.Data.Root.ChannelGroups(2).Channels(4)
oMyResultChn = dd.ChnDurPosInjCalc(oMyXChannel, oMyYChannel, oMyX1Channel, oMyY1Channel, "in one peak (custom)", "Results/LoadDuration", "Results/Amplitude", "Results/Injury", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name)
```

```python
oMyResultChn = dd.ChnDurPosInjCalc("[2]/[1]","[2]/[2]", "[2]/[3]", "[2]/[4]", "in one peak", "Results/LoadDuration", "Results/Amplitude", "Results/Injury")
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name)
```

---

*Source: `ComOff/ChnDurPosInjCalc.htm`*

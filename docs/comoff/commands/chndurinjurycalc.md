---
title: "ChnDurInjuryCalc"
description: "Calculates the time-at-level and the injury risk. The time at level describes the maximum continuous time interval in which the amplitude value of a signal exce"
---

# ChnDurInjuryCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDurInjuryCalc

Calculates the time-at-level and the injury risk. The time at level describes the maximum continuous time interval in which the amplitude value of a signal exceeds a specific lower threshold.

## Signature

```python
return_value = dd.ChnDurInjuryCalc( X , Y , X1 , Y1 , X2 , Y2 , DurationType, ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , CalcSteps, CalcDuration)
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
<td>Specifies the data channel containing the time values of the signal in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel containing the time values of the positive limit curve.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the amplitude values of the positive limit curve.</td></tr>
<tr><td width="150"><em>X2</em></td>
<td>Specifies the data channel containing the time values of the negative limit curve.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel containing the amplitude values of the negative limit curve.</td></tr>
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
<td>Specifies the result channel for the time values of the positive amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the time values of the negative amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the load durations of the positive amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the positive amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the load durations of the negative amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the negative amplitudes.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the positive part of the injury risks.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the negative part of the injury risks.</td></tr>
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
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyX1Channel = dd.Data.Root.ChannelGroups(1).Channels(3)
oMyY1Channel = dd.Data.Root.ChannelGroups(1).Channels(4)
oMyX2Channel = dd.Data.Root.ChannelGroups(1).Channels(5)
oMyY2Channel = dd.Data.Root.ChannelGroups(1).Channels(6)
oMyResultChn = dd.ChnDurInjuryCalc(oMyXChannel, oMyYChannel, oMyX1Channel, oMyY1Channel, oMyX2Channel, oMyY2Channel, "in one peak (custom)", "Results/TimePositiveAmplitudes", "Results/TimeNegativeAmplitudes", "Results/PositiveAmplitudeDuration", "Results/NegativeAmplitudeDuration", "Results/PositiveLoadDuration", "Results/NegativeLoadDuration", "Results/PositiveAmplitude", "Results/NegativeAmplitude", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name , "\r\n" ,"Result channel(4): " , oMyResultChn(4).ChannelGroup.Name , "/" , oMyResultChn(4).Name , "\r\n" ,"Result channel(5): " , oMyResultChn(5).ChannelGroup.Name , "/" , oMyResultChn(5).Name , "\r\n" ,"Result channel(6): " , oMyResultChn(6).ChannelGroup.Name , "/" , oMyResultChn(6).Name , "\r\n" ,"Result channel(7): " , oMyResultChn(7).ChannelGroup.Name , "/" , oMyResultChn(7).Name , "\r\n" ,"Result channel(8): " , oMyResultChn(8).ChannelGroup.Name , "/" , oMyResultChn(8).Name)
```

```python
oMyResultChn = dd.ChnDurInjuryCalc("[1]/[1]", "[1]/[2]", "[1]/[3]", "[1]/[4]", "[1]/[5]", "[1]/[6]", "in one peak (custom)", "Results/TimePositiveAmplitudes", "Results/TimeNegativeAmplitudes", "Results/PositiveAmplitudeDuration", "Results/NegativeAmplitudeDuration", "Results/PositiveLoadDuration", "Results/NegativeLoadDuration", "Results/PositiveAmplitude", "Results/NegativeAmplitude", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name , "\r\n" ,"Result channel(4): " , oMyResultChn(4).ChannelGroup.Name , "/" , oMyResultChn(4).Name , "\r\n" ,"Result channel(5): " , oMyResultChn(5).ChannelGroup.Name , "/" , oMyResultChn(5).Name , "\r\n" ,"Result channel(6): " , oMyResultChn(6).ChannelGroup.Name , "/" , oMyResultChn(6).Name , "\r\n" ,"Result channel(7): " , oMyResultChn(7).ChannelGroup.Name , "/" , oMyResultChn(7).Name , "\r\n" ,"Result channel(8): " , oMyResultChn(8).ChannelGroup.Name , "/" , oMyResultChn(8).Name)
```

---

*Source: `ComOff/ChnDurInjuryCalc.htm`*

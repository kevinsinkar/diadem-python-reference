---
title: "ChnDurPosNegCalc"
description: "Specifies the time-at-level for positive and for negative values. The time at level describes the maximum continuous time interval in which the amplitude value "
---

# ChnDurPosNegCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDurPosNegCalc

Specifies the time-at-level for positive and for negative values. The time at level describes the maximum continuous time interval in which the amplitude value of a signal exceeds a specific lower threshold.

## Signature

```python
return_value = dd.ChnDurPosNegCalc( X , Y , DurationType, ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , ResultChannel , CalcSteps, CalcDuration)
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
<td>Contains six result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyResultChn = dd.ChnDurPosNegCalc(oMyXChannel, oMyYChannel, "in one peak (custom)", "Results/PositiveAmplitudeDuration", "Results/NegativeAmplitudeDuration", "Results/PositiveLoadDuration", "Results/NegativeLoadDuration", "Results/PositiveAmplitude", "Results/NegativeAmplitude", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name , "\r\n" ,"Result channel(4): " , oMyResultChn(4).ChannelGroup.Name , "/" , oMyResultChn(4).Name , "\r\n" ,"Result channel(5): " , oMyResultChn(5).ChannelGroup.Name , "/" , oMyResultChn(5).Name , "\r\n" ,"Result channel(6): " , oMyResultChn(6).ChannelGroup.Name , "/" , oMyResultChn(6).Name)
```

```python
oMyResultChn = dd.ChnDurPosNegCalc("[1]/[1]","[1]/[2]", "in one peak (cusotm)", "Results/PositiveAmplitudeDuration", "Results/NegativeAmplitudeDuration", "Results/PositiveLoadDuration", "Results/PositiveAmplitude", "Results/NegativeLoadDuration", "Results/NegativeAmplitude", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name , "\r\n" ,"Result channel(3): " , oMyResultChn(3).ChannelGroup.Name , "/" , oMyResultChn(3).Name , "\r\n" ,"Result channel(4): " , oMyResultChn(4).ChannelGroup.Name , "/" , oMyResultChn(4).Name , "\r\n" ,"Result channel(5): " , oMyResultChn(5).ChannelGroup.Name , "/" , oMyResultChn(5).Name , "\r\n" ,"Result channel(6): " , oMyResultChn(6).ChannelGroup.Name , "/" , oMyResultChn(6).Name)
```

---

*Source: `ComOff/ChnDurPosNegCalc.htm`*

---
title: "ChnDurPosCalc"
description: "Calculates the time at level. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific threshold."
---

# ChnDurPosCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnDurPosCalc

Calculates the time at level. The time at level describes the maximum continuous time interval in which the amplitude of a signal exceeds a specific threshold.

## Signature

```python
return_value = dd.ChnDurPosCalc( X , Y , DurationType, ResultChannel , ResultChannel , CalcSteps, CalcDuration)
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
<td>Contains two result channels. The first result channel contains the load duration and the second result channel contains the amplitudes. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChannel = dd.Data.Root.ChannelGroups(1).Channels(1)
oMyYChannel = dd.Data.Root.ChannelGroups(1).Channels(2)
oMyResultChn = dd.ChnDurPosCalc(oMyXChannel, oMyYChannel, "in one peak (custom)", "Results/LoadDuration", "Results/Amplitude", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

```python
oMyResultChn = dd.ChnDurposCalc("[1]/[1]","[1]/[2]", "in one peak", "Results/LoadDuration", "Results/Amplitude", 100, 60)
print("Result channel(1): " , oMyResultChn(1).ChannelGroup.Name , "/" , oMyResultChn(1).Name , "\r\n" ,"Result channel(2): " , oMyResultChn(2).ChannelGroup.Name , "/" , oMyResultChn(2).Name)
```

---

*Source: `ComOff/ChnDurPosCalc.htm`*

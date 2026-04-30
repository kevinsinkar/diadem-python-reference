---
title: "ChnEventPatternFind"
description: "Searches for a pattern in a signal."
---

# ChnEventPatternFind

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEventPatternFind

Searches for a pattern in a signal.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. If the associated y-channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the signal to be inspected.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel with the pattern you are looking for.</td></tr>
<tr><td width="150">PatternFindBandwidth</td>
<td>Specifies the maximum number of values by which the signal channel may offset against the pattern channel.<div id="exp_PatternFindBandwidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>0 &lt;= PatternFindBandwidth &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PatternFindAlignPattern</td>
<td>Specifies whether DIAdem uses a y-offset.<div id="exp_PatternFindAlignPattern">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">PatternFindMaxDistance</td>
<td>Specifies the maximum valid deviation of the signal channel to the pattern channel.<div id="exp_PatternFindMaxDistance">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= PatternFindMaxDistance &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150"><em>[ResultChannel]</em></td>
<td>Specifies, whether DIAdem generates a result channel containing the minimal deviations of the signal from the pattern for each point of the signal.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Variant</a> type. A return value is a two-dimensional array containing the search results. Refer to <a href="#" data-unresolved="1">Result of the Event Search</a> for a detailed description of the array. The generated data matrix contains the index 0 to index 7 in the second dimension. The index 0 and index 1 contain the start and end indexes of the wanted event. If you specify a waveform channel as the y-channel or if you specify an x-channel explicitly for the pattern search in the input parameter <span class="Monospace">SourceChn</span>, index 2 and index 3 contain the start and end x-values otherwise the values are <span class="Monospace">Null</span>. Index 4 and index 5 contain the start and end y-values of the inspected signals. Index 6 contains the deviation of the signal channel to the pattern channel.<br attr="ext"/>Use the variables <a href="../../../varoff/variables/chneventlist1/">ChnEventList1</a>, <a href="../../../varoff/variables/chneventlist2/">ChnEventList2</a>, or <a href="../../../varoff/variables/chneventresultlist/">ChnEventResultList</a> as the return value of this function or define your own variable.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnEventPatternFind.htm`*

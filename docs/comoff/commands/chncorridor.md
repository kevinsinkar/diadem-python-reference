---
title: "ChnCorridor"
description: "Calculates two curves which have a fixed distance to the input signal. All points of the input signal and the connection line between two consecutive points are"
---

# ChnCorridor

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCorridor

Calculates two curves which have a fixed distance to the input signal. All points of the input signal and the connection line between two consecutive points are in the band formed by the result channels.

## Signature

```python
return_value = dd.ChnCorridor( XW , Y , ResultChannel , ResultChannel , ResultChannel , CorridorOffsetYType, CorridorOffsetYValue, [CorridorOffsetXType], [CorridorOffsetXValue], [CorridorPointsPerLine], [CorridorPointsPerArc])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values. If the associated channel is a waveform or xy-channel, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the parallel curves.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the upper parallel curve.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the lower parallel curve.</td></tr>
<tr><td width="150">CorridorOffsetYType</td>
<td>Specifies whether the distance of the parallel curves to the input signal in y-direction is specified in absolute or relative numbers.<div id="exp_CorridorOffsetYType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"relativeYScale"</pre></donottranslate></td>
<td>Relative in y-area</td></tr>
<tr><td width="150"><donottranslate><pre>"relativeXScale"</pre></donottranslate></td>
<td>Relative in x-area</td></tr>
<tr><td width="150"><donottranslate><pre>"absoluteScale"</pre></donottranslate></td>
<td>Absolute</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">CorridorOffsetYValue</td>
<td>Specifies the distance of the parallel curves to the input signal in y-direction.<div id="exp_CorridorOffsetYValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>1E-9 &lt;= CorridorOffsetYValue &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[CorridorOffsetXType]</td>
<td>Specifies whether the distance of the parallel curves to the input signal in x-direction is specified in absolute or relative numbers.<div id="exp_CorridorOffsetXType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"sameAsY"</pre></donottranslate></td>
<td>Like in y-direction</td></tr>
<tr><td width="150"><donottranslate><pre>"relativeXScale"</pre></donottranslate></td>
<td>Relative in x-area</td></tr>
<tr><td width="150"><donottranslate><pre>"relativeYScale"</pre></donottranslate></td>
<td>Relative in y-area</td></tr>
<tr><td width="150"><donottranslate><pre>"absoluteScale"</pre></donottranslate></td>
<td>Absolute</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[CorridorOffsetXValue]</td>
<td>Specifies the distance of the parallel curves to the input signal in x-direction.<div id="exp_CorridorOffsetXValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0 &lt;= CorridorOffsetXValue &lt;= 1E300<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[CorridorPointsPerLine]</td>
<td>Specifies the number of extra partitions between two points of the input signal. A greater number of partitions creates curves that adjust better to the signal, especially with greater distances, but this also needs more computing time.<div id="exp_CorridorPointsPerLine">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>0 &lt;= CorridorPointsPerLine &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[CorridorPointsPerArc]</td>
<td>Specifies the number of extra curve partitions at the local extreme values of the input signal. A greater number of partitions creates smoother curves but also needs more computing time.<div id="exp_CorridorPointsPerArc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>1 &lt;= CorridorPointsPerArc &lt;= 2147483647<br attr="ext"/>Access: Read/Write</td></tr>
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

---

*Source: `ComOff/ChnCorridor.htm`*

---
title: "ChnASICalc"
description: "Calculates the Acceleration Severity Index (ASI). The ASI value determines the effect vehicle acceleration has on a person sitting near a certain point at the t"
---

# ChnASICalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnASICalc

Calculates the Acceleration Severity Index (ASI). The ASI value determines the effect vehicle acceleration has on a person sitting near a certain point at the time of impact.

## Signature

```python
return_value = dd.ChnASICalc( XW , X1 , Y1 , Z1 , ResultChannel , ASIDelta, [ASIFilterType])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you want to use waveform channels in this command follow <a href="#" data-unresolved="1">rules 2.2 and 2.3 for calculating with waveform channels</a>.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the results and the version number, which differs from the DIAdem version number, in the following custom properties of the result channel: <span class="Monospace">ResultASIMax</span> and <span class="Monospace">ResultASIVersion</span>.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The sampling interval of the time channel must be smaller than the value set for the length of the time interval.<p class="body">The calculation filters data using a CFC filter with a 13 Hz limit frequency in accordance with the norm EN 1317-1:2010, or calculates a moving mean of the data according to the older norm EN 1317-1:1998, depending on which settings you make. According to EN 1317-2, Chapter 5.6, the input channels must be additionally filtered with CFC180.</p>
</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the standard EN 1317-1, Road Restraint Systems, Part 1 Terminology and General Criteria for Test Methods, for more information about this crash function.</td>
</tr>
</table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the description of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds.</td></tr>
<tr><td width="150"><em>X1</em></td>
<td>Specifies the data channel containing the x-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the y-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>Z1</em></td>
<td>Specifies the data channel containing the z-acceleration values in gn (gravity acceleration).</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">ASIDelta</td>
<td>Specifies the length of the time interval in ms for the calculation of the moving average in the ASI calculation.<div id="exp_ASIDelta">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ASIDelta &lt;= 1E300</td></tr>
</table>
<p class="body">Recommended value: 50 ms.</p>
</div></td></tr>
<tr><td width="150">[ASIFilterType]</td>
<td>Specifies the method of filtering in the ASI calculation. If you do not set this parameter, DIAdem filters with a moving average calculation.<div id="exp_ASIFilterType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"MovingAverage"</pre></donottranslate></td>
<td>Moving average(EN 1317-1:1998)</td></tr>
<tr><td width="150"><donottranslate><pre>"CFC_CFR13"</pre></donottranslate></td>
<td>CFC filter with CFR=13Hz (EN 1317-1:2010)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnASICalc.htm`*

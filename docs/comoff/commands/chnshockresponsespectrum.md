---
title: "ChnShockResponseSpectrum"
description: "Calculates the shock response spectrum (SRS) from an acceleration signal. The calculation is executed in accordance with ISO-Norm 18431-4:2007. The shock respon"
---

# ChnShockResponseSpectrum

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnShockResponseSpectrum

Calculates the shock response spectrum (SRS) from an acceleration signal. The calculation is executed in accordance with ISO-Norm 18431-4:2007. The shock response spectrum describes the response to the acceleration of many single-degree-of-freedom systems which is a mass-damping-spring system with different natural harmonics.

## Signature

```python
return_value = dd.ChnShockResponseSpectrum( XW , Y , ResultChannel , ResultChannel , SRSRangeType, SRSAmplitudeType, SRSResultType, SRSStartFrequency, SRSEndFrequency, SRSFreqPerOctave, SRSDamping, SRSPulseDuration)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The values of the XW-channel (time channel) must be equidistant and monotonic increasing.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the signal values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel with the frequencies.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel determined by the selected result type.</td></tr>
<tr><td width="150">SRSRangeType</td>
<td>Specifies the time domain of the shock event. The start range extends over the pulse duration of the shock event.<div id="exp_SRSRangeType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Primary"</pre></donottranslate></td>
<td>Start range</td></tr>
<tr><td width="150"><donottranslate><pre>"Residual"</pre></donottranslate></td>
<td>Rest range</td></tr>
<tr><td width="150"><donottranslate><pre>"All"</pre></donottranslate></td>
<td>Complete range</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRSAmplitudeType</td>
<td>Specifies the amplitude type of the shock response spectrum.<div id="exp_SRSAmplitudeType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"AmpMaxiMax"</pre></donottranslate></td>
<td>Absolute maxima</td></tr>
<tr><td width="150"><donottranslate><pre>"AmpMaxNegative"</pre></donottranslate></td>
<td>Minimum values</td></tr>
<tr><td width="150"><donottranslate><pre>"AmpMaxPositive"</pre></donottranslate></td>
<td>Maximum values</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRSResultType</td>
<td>Specifies the result type of the shock response spectrum.<div id="exp_SRSResultType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Acceleration"</pre></donottranslate></td>
<td>Acceleration</td></tr>
<tr><td width="150"><donottranslate><pre>"RelativeVelocity"</pre></donottranslate></td>
<td>Relative velocity</td></tr>
<tr><td width="150"><donottranslate><pre>"RelativeDisplacement"</pre></donottranslate></td>
<td>Relative displacement</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRSStartFrequency</td>
<td>Specifies the start frequency of the shock response spectrum.<div id="exp_SRSStartFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SRSStartFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRSEndFrequency</td>
<td>Specifies the end frequency of the shock response spectrum.<div id="exp_SRSEndFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SRSEndFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SRSFreqPerOctave</td>
<td>Specifies the number of frequencies per octave of the shock response spectrum.<div id="exp_SRSFreqPerOctave">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= SRSFreqPerOctave &lt;= 2147483647</td></tr>
</table>
<p>The frequency distribution is logarithmic. Use the following formula to calculate the n frequency:<br attr="ext"/><img src="image/SRS_frequence.gif"/></p>
</div></td></tr>
<tr><td width="150">SRSDamping</td>
<td>Specifies the damping degree of the single-degree-of-freedom systems.<div id="exp_SRSDamping">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SRSDamping &lt;= 1</td></tr>
</table>
<p>Use the following formula to calculate the damping degree:<br attr="ext"/><img src="image/SRS_damping.gif"/><br attr="ext"/>Q specifies the quality.</p>
</div></td></tr>
<tr><td width="150">SRSPulseDuration</td>
<td>Specifies the pulse duration of the shock response. If you specify <span class="Monospace">0</span>, the pulse duration is valid for the entire measurement.<div id="exp_SRSPulseDuration">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SRSPulseDuration &lt;= 1E300</td></tr>
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

*Source: `ComOff/ChnShockResponseSpectrum.htm`*

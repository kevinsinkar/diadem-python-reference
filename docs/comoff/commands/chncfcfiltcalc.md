---
title: "ChnCFCFiltCalc"
description: "Executes digital phaseless filtering of a signal according to SAE J211."
---

# ChnCFCFiltCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnCFCFiltCalc

Executes digital phaseless filtering of a signal according to SAE J211.

## Signature

```python
return_value = dd.ChnCFCFiltCalc( XW , Y , ResultChannel , CFCFiltType, [Fir100RemoveBias], [CFCPreEventType], [CFCFreeValue])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you want to use waveform channels in this command follow <a href="#" data-unresolved="1">rules 2.2 and 2.3 for calculating with waveform channels</a>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">CFC Filter</a> for further information such as mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the amplitude values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">CFCFiltType</td>
<td>Specifies the filtering characteristic with specific limit frequencies and tolerance widths for lowpass filters.<div id="exp_CFCFiltType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"CFC_60"</pre></donottranslate></td>
<td>CFC 60 filters</td></tr>
<tr><td width="150"><donottranslate><pre>"CFC_180"</pre></donottranslate></td>
<td>CFC 180 filters</td></tr>
<tr><td width="150"><donottranslate><pre>"CFC_600"</pre></donottranslate></td>
<td>CFC 600 filters</td></tr>
<tr><td width="150"><donottranslate><pre>"CFC_1000"</pre></donottranslate></td>
<td>CFC 1000 filters</td></tr>
<tr><td width="150"><donottranslate><pre>"FIR_100"</pre></donottranslate></td>
<td>FIR 100 filters</td></tr>
<tr><td width="150"><donottranslate><pre>"CFC_Free"</pre></donottranslate></td>
<td>CFC any</td></tr>
</table>
</td></tr>
</table>
<h2>Valid settings</h2>
<table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" id="AutoNumber1" style="border-collapse: collapse">
<tr>
<td width="150">CFC_60</td>
<td>3-dB limit frequency: 100 Hz, stop damping: -30 dB</td>
</tr>
<tr>
<td width="150">CFC_180</td>
<td>3-dB limit frequency: 300 Hz, stop damping: -30 dB</td>
</tr>
<tr>
<td width="150">CFC_600</td>
<td>3-dB limit frequency: 1000 Hz, stop damping: -40 dB</td>
</tr>
<tr>
<td width="150">CFC_1000</td>
<td>3-dB limit frequency: 1650 Hz, stop damping: -40 dB</td>
</tr>
<tr>
<td width="150">FIR_100</td>
<td>CFC_180 unphased, Subsampling to 1600 Hz , elimination of bias, 3-dB limit frequency: Hertz, Stop damping: -50 dB, Oversampling</td>
</tr>
<tr>
<td width="150">CFC_Free</td>
<td>Non-standardized filter class with the approximate 3-dB limit frequency <a href="../../../varoff/variables/cfcfreevalue/">CFCFreeValue</a>*1.65</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[Fir100RemoveBias]</td>
<td>Specifies whether DIAdem eliminates the bias in FIR100 filtering. The default value is <span class="Monospace">FALSE</span>, which specifies that DIAdem does not remove the bias.<div id="exp_Fir100RemoveBias">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[CFCPreEventType]</td>
<td>Specifies how DIAdem extends the input data at the starting point and the end point of the signal, to eliminate transient response in the filter. If you do not specify the variable <span class="Monospace">CFCPreEventType</span>, DIAdem uses the value <span class="Monospace">ZeroMagnitude</span>.<div id="exp_CFCPreEventType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"EndPoints"</pre></donottranslate></td>
<td>End points</td></tr>
<tr><td width="150"><donottranslate><pre>"ZeroMagnitude"</pre></donottranslate></td>
<td>Zero amplitude</td></tr>
</table>
</td></tr>
</table>
<p class="Body">If the data of a signal contains enough information about the signal process before the relevant cutoff and after the end point of the digital filtering, the initial condition can be disregarded. If the history of the signal is unknown, you can balance the transients of the filter when you set the start value of the filtered signal to an amplitude of zero or to the first amplitude value of the unfiltered signal. Copy at least 10ms of the original signal data directly before the start point and then execute a rotary reflection at the source of the coordinate system (<span class="Monospace">ZeroMagnitude</span>) or at the start point of the  original signal (<span class="Monospace">Endpoints</span>). Repeat the procedure at the end of the data set. After filtering the extended data set, DIAdem discards the added data areas again.</p>
<p class="Body">Mirroring at the start point of the original signal:</p>
<p class="Body"><img border="0" height="304" src="image/SAEJ21_2.gif" width="433"/></p>
<p class="Body">Mirroring at the original coordinate system:</p>
<p class="Body"><img border="0" height="302" src="image/SAEJ21_1.gif" width="430"/></p>
<p class="Body"></p>
</div></td></tr>
<tr><td width="150">[CFCFreeValue]</td>
<td>Specifies the filter class when the CFC filtering is non-standardized. If you do not specify the <span class="Monospace">CFCFreeValue</span> variable, DIAdem uses the value <span class="Monospace">0</span>.<div id="exp_CFCFreeValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= CFCFreeValue &lt;= 1E300</td></tr>
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

*Source: `ComOff/ChnCFCFiltCalc.htm`*

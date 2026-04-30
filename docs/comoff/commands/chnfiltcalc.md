---
title: "ChnFiltCalc"
description: "Filters a signal digitally."
---

# ChnFiltCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFiltCalc

Filters a signal digitally.

## Signature

```python
return_value = dd.ChnFiltCalc( XW , Y , ResultChannel , FiltStruc, FiltStyle, FiltType, FiltDegree, FiltLimit, FiltLowLimit, FiltUppLimit, FiltWave, FiltSamples, FiltWndFct, FiltZeroPhase, FiltCorrection)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> The maximum filtering degree for Bessel filters is ten.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If you want to use waveform channels in this command follow <a href="#" data-unresolved="1">rules 2.2 and 2.3 for calculating with waveform channels</a>.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">FiltStruc</td>
<td>Specifies the filter method.<div id="exp_FiltStruc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"IIR"</pre></donottranslate></td>
<td>IIR filter</td></tr>
<tr><td width="150"><donottranslate><pre>"FIR"</pre></donottranslate></td>
<td>FIR filter</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">FiltStyle</td>
<td>Specifies the filter type when an IIR filter method is used.<div id="exp_FiltStyle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Bessel"</pre></donottranslate></td>
<td>Bessel filters</td></tr>
<tr><td width="150"><donottranslate><pre>"Butterworth"</pre></donottranslate></td>
<td>Butterworth filters</td></tr>
<tr><td width="150"><donottranslate><pre>"Chebyshev"</pre></donottranslate></td>
<td>Chebyshev filters</td></tr>
</table>
</td></tr>
</table>
<h2>Valid Settings</h2>
<table border="0" bordercolor="#111111" cellpadding="0" cellspacing="0" id="AutoNumber1" style="border-collapse: collapse">
<tr>
<td width="150"><donottranslate><pre>Bessel</pre></donottranslate></td>
<td>
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">The Bessel filter has good rectangle transition behavior, and little tendency to overshoot. The transition from the pass-through domain to the block domain is relatively flat.  The Bessel filter has a linear phase response in the time-continuous domain.</p>
</td>
</tr>
<tr>
<td width="150"><donottranslate><pre>Butterworth</pre></donottranslate></td>
<td>
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">The Butterworth filter has a steep transition from the pass-through to the block domain.</p>
</td>
</tr>
<tr>
<td width="150"><donottranslate><pre>Chebyshev</pre></donottranslate></td>
<td>
<p class="Body" style="margin-top: 1pt; margin-bottom: 1pt">The Chebyshev filter has a steep transition from the pass-through to the block band. The Chebyshev filter has a strong waviness in the pass-band.</p>
</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">FiltType</td>
<td>Specifies the filter type.<div id="exp_FiltType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Low pass"</pre></donottranslate></td>
<td>Lowpass</td></tr>
<tr><td width="150"><donottranslate><pre>"High pass"</pre></donottranslate></td>
<td>Highpass</td></tr>
<tr><td width="150"><donottranslate><pre>"Band pass"</pre></donottranslate></td>
<td>Bandpass</td></tr>
<tr><td width="150"><donottranslate><pre>"Band stop"</pre></donottranslate></td>
<td>Bandstop</td></tr>
<tr><td width="150"><donottranslate><pre>"All pass"</pre></donottranslate></td>
<td>Allpass</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">FiltDegree</td>
<td>Specifies the filter degree for digital filtering with IIR filters.<div id="exp_FiltDegree">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>1 &lt;= FiltDegree &lt;= 16</td></tr>
</table>
<p class="Body">The filtering degree is a unit for the quality of the IIR filter, and also specifies the maximum phase rotation and the number of back tracking filter output signals. The higher the filtering degree you select, the smaller the transfer band width, which means the transition from the pass range to the stop range is correspondingly steeper. High degree filters are cascade switches of first or second degree filters.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note </strong> The maximum filtering degree for Bessel filters is ten.</td></tr></table>
</div></td></tr>
<tr><td width="150">FiltLimit</td>
<td>Specifies the 3 dB limit frequency of an IIR filter for highpass and lowpass. For allpass of an FIR filter, it specifies the frequency where the phase angle rotation reaches half the phase angle rotation of the overall system.<div id="exp_FiltLimit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= FiltLimit &lt;= 1E300</td></tr>
</table>
<p>For digital filtering, DIAdem sets the limit frequencies according to the filtering type. The limit frequencies define which frequency domains are blocked and which frequency domains constitute the pass band.</p>
</div></td></tr>
<tr><td width="150">FiltLowLimit</td>
<td>Specifies the lower 3 dB-limit frequency for bandpass or bandstop.<div id="exp_FiltLowLimit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= FiltLowLimit &lt;= 1E300</td></tr>
</table>
<p class="Body">If you use an IIR filter and one of the filter types bandpass or bandstop, you specify the lower 3 dB limit frequency with the parameter  <span class="Monospace">FiltLowLimit</span>. If you use an FIR filter, the frequency response has the value 0.5 at this point.</p>
</div></td></tr>
<tr><td width="150">FiltUppLimit</td>
<td>Specifies the upper 3 dB-limit frequency for bandpass or bandstop.<div id="exp_FiltUppLimit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= FiltUppLimit &lt;= 1E300</td></tr>
</table>
<p class="Body">If you use an IIR filter and one of the filter types bandpass or bandstop, you specify the upper 3 dB limit frequency with the parameter  <span class="Monospace">FiltUppLimit</span>. If you use an FIR filter, the frequency response has the value 0.5 at this point.</p>
</div></td></tr>
<tr><td width="150">FiltWave</td>
<td>Specifies the ripple in the pass range for Chebyshev filtering.<div id="exp_FiltWave">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0.01 &lt;= FiltWave &lt;= 3</td></tr>
</table>
</div></td></tr>
<tr><td width="150">FiltSamples</td>
<td>Specifies the number of values in the input signal that DIAdem calculates in linear filter structure.<div id="exp_FiltSamples">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>2 &lt;= FiltSamples &lt;= 10000</td></tr>
</table>
</div></td></tr>
<tr><td width="150">FiltWndFct</td>
<td>Specifies the window functions when DIAdem uses non-recursive FIR filters.<div id="exp_FiltWndFct">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Rectangle"</pre></donottranslate></td>
<td>Rectangle</td></tr>
<tr><td width="150"><donottranslate><pre>"Hanning"</pre></donottranslate></td>
<td>Hanning</td></tr>
<tr><td width="150"><donottranslate><pre>"Hamming"</pre></donottranslate></td>
<td>Hamming</td></tr>
<tr><td width="150"><donottranslate><pre>"Blackman"</pre></donottranslate></td>
<td>Blackman</td></tr>
<tr><td width="150"><donottranslate><pre>"Bartlett"</pre></donottranslate></td>
<td>Bartlett</td></tr>
<tr><td width="150"><donottranslate><pre>"Mod.rectangle"</pre></donottranslate></td>
<td>Modified rectangle</td></tr>
</table>
</td></tr>
</table>
<p class="Body">If you filter a signal with non-recursive FIR filters digitally, DIAdem limits and weights the infinite impulse response with the window function specified here.</p>
</div></td></tr>
<tr><td width="150">FiltZeroPhase</td>
<td>Specifies whether DIAdem eliminates phase shifting in the filtered signal when IIR filters are used.<div id="exp_FiltZeroPhase">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If you force the zero phase, the signal traverses the filter algorithm once forward and then backwards. The imaginary part of the transfer function receives the value zero, which indicates the the phase shifting is eliminated.</p>
<p class="Body">Internally the program calculates with half the order so that DIAdem reaches the specified filter order. The double filtering process compensates this. Therefore you only can specify even-numbered filter orders.</p>
</div></td></tr>
<tr><td width="150">FiltCorrection</td>
<td>Specifies whether DIAdem corrects the offset for lowpass filters when it runs digital filtering on a time signal with recursive IIR filters.<div id="exp_FiltCorrection">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">An offset correction is necessary if false signals arise as a result of a vibration constraint process when the initial amplitude is not equal to zero. DIAdem reduces the entire signal by the size of the initial amplitude, before the filtering process starts. This means DIAdem shifts the signal to the zero point. After the filtering procedure DIAdem adds the offset again to the filtered signal.</p>
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

*Source: `ComOff/ChnFiltCalc.htm`*

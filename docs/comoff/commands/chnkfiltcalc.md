---
title: "ChnKFiltCalc"
description: "Analyzes mechanical vibrations that effect the human body in manifold ways, for example, at the workplace or in vehicles."
---

# ChnKFiltCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnKFiltCalc

Analyzes mechanical vibrations that effect the human body in manifold ways, for example, at the workplace or in vehicles.

## Signature

```python
dd.ChnKFiltCalc( XW , Y , KFiltType, KFiltOscillation, KFiltAverageTime, KFiltRedFactor, KFiltNorm)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For hand-arm vibrations, the sampling frequency must be higher than 1000 Hz, in other cases it must be higher than 200 Hz.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal.</td></tr>
<tr><td width="150">KFiltType</td>
<td>Specifies the frequency weighting filter for time-related body and hand-arm vibrations.<div id="exp_KFiltType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"KX"</pre></donottranslate></td>
<td>KX</td></tr>
<tr><td width="150"><donottranslate><pre>"KY"</pre></donottranslate></td>
<td>KY</td></tr>
<tr><td width="150"><donottranslate><pre>"KZ"</pre></donottranslate></td>
<td>KZ</td></tr>
<tr><td width="150"><donottranslate><pre>"KXL"</pre></donottranslate></td>
<td>KXL</td></tr>
<tr><td width="150"><donottranslate><pre>"KYL"</pre></donottranslate></td>
<td>KYL</td></tr>
<tr><td width="150"><donottranslate><pre>"KZL"</pre></donottranslate></td>
<td>KZL</td></tr>
<tr><td width="150"><donottranslate><pre>"KB"</pre></donottranslate></td>
<td>KB</td></tr>
<tr><td width="150"><donottranslate><pre>"KH"</pre></donottranslate></td>
<td>KH</td></tr>
</table>
</td></tr>
</table>
<p class="Body">The k-evaluated signal is the result of frequency evaluation and normalizing of the unevaluated, time-dependent acceleration signal. The unit of the acceleration signal must be m/s². The result is not dimensioned after normalization.</p>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>For hand-arm vibrations, the sampling frequency must be higher than 1000 Hz, in other cases it must be higher than 200 Hz.</td></tr></table>
<p class="Body">In compliance with DIN 45671, part 1 the evaluation filter must be used as follows:</p>
<table class="borderlessborder">
<tr><td width="150">KX, KY, KZ</td>
<td>for standing and seated positions in the x, y and z-measurement directions</td></tr>
<tr><td width="150">KXL, KYL, KZL</td>
<td>for prostrate positions in the x, y and z-measurement directions</td></tr>
<tr><td width="150">KB</td>
<td>for non-specified body position</td></tr>
<tr><td width="150">KH</td>
<td>for hand-arm vibrations and all measurement directions</td></tr>
</table>
</div></td></tr>
<tr><td width="150">KFiltOscillation</td>
<td>Specifies whether DIAdem calculates the weighted oscillation severity.<div id="exp_KFiltOscillation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If DIAdem does not calculate the mean value, a <a href="../../../varoff/variables/kfiltredfactor/">Data reduction</a> is not possible. The exponential mean is calculated with the following recursion equation:</p>
<pre><donottranslate>MW_k+1 = sqrt((1-F)*MW_ky² + F*Y_ky² ) </donottranslate></pre>
<p class="Body">with</p>
<table class="borderlessborder">
<tr><td width="50">MW</td>
<td>Mean channel</td></tr>
<tr><td width="50">y</td>
<td>K-evaluated signal</td></tr>
<tr><td width="50">F</td>
<td>2 / Sampling frequency / Averaging time</td></tr>
</table>
<p class="Body">The factor <em>F</em> must be greater than <span class="Monospace">1</span>. Exponential averaging corresponds to a first order low-pass filter.</p>
</div></td></tr>
<tr><td width="150">KFiltAverageTime</td>
<td>Specifies the time constant for mean calculations, in seconds.<div id="exp_KFiltAverageTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= KFiltAverageTime &lt;= 1E300</td></tr>
</table>
<p class="Body">DIN 45671 (part 1) specifies the values 0.125s (FAST), 1s (SLOW), and 8s (VERYSLOW).</p>
</div></td></tr>
<tr><td width="150">KFiltRedFactor</td>
<td>Specifies that DIAdem reduces the result values to each nth k-value, starting at the first result value.<div id="exp_KFiltRedFactor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= KFiltRedFactor &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
<p class="Body">DIAdem only runs a data reduction together with a <a href="../../../varoff/variables/kfiltoscillation/">Evaluated vibration severity</a>.</p>
</div></td></tr>
<tr><td width="150">KFiltNorm</td>
<td>Specifies whether DIAdem normalizes the k-value calculation.<div id="exp_KFiltNorm">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">To norm the k-evaluated signal, DIAdem multiplies the signal values by the defined acceleration value, which depends on the selected filter type. After the normalization the frequency-weighted acceleration signals are nondimensional in the range <span class="Monospace">-1</span> to <span class="Monospace">+1</span>.</p>
<p class="Body">DIN 45671 Part 1 specifies the following factors ( in 1/(ms²) ):</p>
<table class="Borderless">
<tr><td width="150">KX, KY, KYL, KZL, KB:</td>
<td>1/0.035</td></tr>
<tr><td width="150">KZ:</td>
<td>1/0.05</td></tr>
<tr><td width="150">KXL:</td>
<td>1/0.033</td></tr>
<tr><td width="150">KH:</td>
<td>1/0.016</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">KFiltValMax</td><td>Receives the highest evaluated vibration severity of a k-value analysis.<div id="exp_KFiltValMax">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Python example

```python
dd.ChnKFiltCalc("Group/Chn1","Group/Chn2","KYL",True,0.125,3,False)
```

---

*Source: `ComOff/ChnKFiltCalc.htm`*

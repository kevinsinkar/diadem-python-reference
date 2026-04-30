---
title: "ChnSingleToneExtract"
description: "Specifies the single frequency with the greatest amplitude in the input signal and returns the frequency and the associated amplitude and phase."
---

# ChnSingleToneExtract

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSingleToneExtract

Specifies the single frequency with the greatest amplitude in the input signal and returns the frequency and the associated amplitude and phase.

## Signature

```python
dd.ChnSingleToneExtract( XW , Y , SingleToneSearchFrequency, SingleToneSearchWidth)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the calculated coefficients in the following custom properties of the input channel: <span class="Monospace">Result~SingleTone~Frequency</span>, <span class="Monospace">Result~SingleTone~Amplitude</span>, and <span class="Monospace">Result~SingleTone~Phase</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150">SingleToneSearchFrequency</td>
<td>Specifies the approximate center frequency which DIAdem uses to search for the fundamental frequency in the frequency domain. If the value is <span class="Monospace">-1</span>, DIAdem uses the frequency with the greatest amplitude as fundamental frequency.<div id="exp_SingleToneSearchFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-1 &lt;= SingleToneSearchFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SingleToneSearchWidth</td>
<td>Specifies the relative frequency width to search for the fundamental frequency in the frequency domain. Specify the frequency width as a percentage of the sampling rate.<div id="exp_SingleToneSearchWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SingleToneSearchWidth &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150">SingleToneFrequency</td><td>Receives the frequency with the greatest amplitude in the input signal.<div id="exp_SingleToneFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SingleToneFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr><tr><td width="150">SingleToneAmplitude</td><td>Receives the greatest amplitude with this single frequency.<div id="exp_SingleToneAmplitude">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SingleToneAmplitude &lt;= 1E300</td></tr>
</table>
</div></td></tr><tr><td width="150">SingleTonePhase</td><td>Receives the phase of this single frequency.<div id="exp_SingleTonePhase">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-360 &lt;= SingleTonePhase &lt;= 360</td></tr>
</table>
</div></td></tr></table>
</div>

---

*Source: `ComOff/ChnSingleToneExtract.htm`*

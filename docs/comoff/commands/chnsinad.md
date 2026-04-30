---
title: "ChnSINAD"
description: "Executes a SINAD analysis (Signal to Noise and Distortion) which specifies the signal-noise interval plus the distortion of a signal. The command determines the"
---

# ChnSINAD

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSINAD

Executes a SINAD analysis (Signal to Noise and Distortion) which specifies the signal-noise interval plus the distortion of a signal. The command determines the basic oscillation and outputs the basic frequency and the SINAD value in decibel.

## Signature

```python
dd.ChnSINAD( XW , Y , SINADSearchFrequency, SINADSearchWidth)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the calculation results in the following custom properties of the input channel: <span class="Monospace">Result~SINAD~DetectedFrequency</span>, <span class="Monospace">Result~SINAD~Value</span>, and <span class="Monospace">Result~SINAD~THDPlusNoise</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150">SINADSearchFrequency</td>
<td>Specifies the approximate center frequency which DIAdem uses to search for the fundamental frequency in the frequency domain. If the value is <span class="Monospace">-1</span>, DIAdem uses the frequency with the greatest amplitude as fundamental frequency.<div id="exp_SINADSearchFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-1 &lt;= SINADSearchFrequency &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SINADSearchWidth</td>
<td>Specifies the relative frequency width to search for the fundamental frequency in the frequency domain. Specify the frequency width as a percentage of the sampling rate.<div id="exp_SINADSearchWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SINADSearchWidth &lt;= 1E300</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150">SINADResult</td>
<td>Receives the SINAD value (signal to noise and distortion). The SINAD value specifies the signal to distortion ratio in dB. The ratio is defined as the ratio of the effective energy of the input signal to the effective energy of the input signal less the energy of the fundamental frequency.<div id="exp_SINADResult">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SINADResult &lt;= 1E300</td></tr>
</table></div></td></tr>
<tr><td width="150">SINADDetectedFrequency</td><td>Receives the fundamental frequency of the signal.<div id="exp_SINADDetectedFrequency">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SINADDetectedFrequency &lt;= 1E300</td></tr>
</table></div></td>
</tr>
<tr><td width="150">SINADTHDPlusNoise</td>
<td>Receives the distortion plus noise. You calculate the distortion by multiplying the SINAD value in decibel with -1.<div id="exp_SINADTHDPlusNoise">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= SINADTHDPlusNoise &lt;= 1</td></tr>
</table></div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnSINAD.htm`*

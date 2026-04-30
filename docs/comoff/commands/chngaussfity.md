---
title: "ChnGaussFitY"
description: "Calculates a Gaussian curve fitting with the least square method, the least residual method, or the bisquare method."
---

# ChnGaussFitY

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGaussFitY

Calculates a Gaussian curve fitting with the least square method, the least residual method, or the bisquare method.

## Signature

```python
dd.ChnGaussFitY( XW , Y , SamplingPointChn, ResultChannel , GaussFitTolerance, GaussFitAlgorithm)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong> DIAdem stores the calculated coefficients and the residual in the following custom properties of the result channels: <span class="Monospace">Result~GaussFit~Amplitude</span> , <span class="Monospace">Result~GaussFit~Center</span> , <span class="Monospace">Result~GaussFit~StandardDeviation</span>, and <span class="Monospace">Result~GaussFit~Residue</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150">SamplingPointChn</td>
<td>Specifies the data channel containing the interpolation points.<div id="exp_SamplingPointChn">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the approximation function.</td></tr>
<tr><td width="150">GaussFitTolerance</td>
<td>Specifies the tolerance that specifies when to end the iterative fit of the amplitude, the center, and the standard deviation in the bisquare method for a Gaussian curve fitting. If the relative difference of the residual undershoots the tolerance in two successive cycles, the curve fitting stops. If the tolerance is 0, DIAdem sets the tolerance to 0.0001.<div id="exp_GaussFitTolerance">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= GaussFitTolerance &lt;= 1E300</td></tr>
</table>
</div></td></tr>
<tr><td width="150">GaussFitAlgorithm</td>
<td>Specifies the algorithm for Gaussian curve fitting.<div id="exp_GaussFitAlgorithm">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Least Square"</pre></donottranslate></td>
<td>Least squares</td></tr>
<tr><td width="150"><donottranslate><pre>"Least Absolute Residual"</pre></donottranslate></td>
<td>Least absolute residual</td></tr>
<tr><td width="150"><donottranslate><pre>"Bisquare"</pre></donottranslate></td>
<td>Bisquare</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table16"><tr><td width="150">GaussFitAmplitude</td><td>Receives the amplitude of the Gaussian curve fitting.<div id="exp_GaussFitAmplitude">
<table class="Borderless" id="table17">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr><tr><td width="150">GaussFitCenter</td><td>Receives the center of the Gaussian curve fitting.<div id="exp_GaussFitCenter">
<table class="Borderless" id="table18">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr><tr><td width="150">GaussFitStdDev</td><td>Receives the standard deviation of the Gaussian curve fitting.<div id="exp_GaussFitStdDev">
<table class="Borderless" id="table19">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr><tr><td width="150">GaussFitResidue</td><td>Receives the residue or the weighted mean error of a Gaussian curve fitting. If you select the <span class="Monospace">Least absolute residual</span> algorithm, the variable receives the absolute error of the weighted mean. If you use other algorithms, the variable does not receive an absolute value.<div id="exp_GaussFitResidue">
<table class="Borderless" id="table20">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr></table>
</div>

---

*Source: `ComOff/ChnGaussFitY.htm`*

---
title: "ChnAkimaYCalc"
description: "Approximates a signal with an Akima subspline."
---

# ChnAkimaYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnAkimaYCalc

Approximates a signal with an Akima subspline.

## Signature

```python
return_value = dd.ChnAkimaYCalc( XW , Y , SamplingPointChn, ResultChannel , AkimaFit, AkimaRange, AkimaCoeff, AkimaPerc)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you assign the value zero to the <span class="Monospace">AkimaPerc</span> variable, DIAdem does not limit the interpolation points.</td></tr></table>
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
<td>Specifies the result channel containing the y-values of the spline function.</td></tr>
<tr><td width="150">AkimaFit</td>
<td>Specifies whether DIAdem uses an interpolating or an approximating curve type for Akima subsplines.<div id="exp_AkimaFit">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
<p class="Body">If you select an interpolating curve type, DIAdem adopts the y-interpolation points of the output signal. If you select an approximating curve type, DIAdem approximates the specified y-interpolation points by averaging the original values and their neighboring interpolation points. This allows you to relativize errors in individual measured points.</p>
</div></td></tr>
<tr><td width="150">AkimaRange</td>
<td>Specifies the number of neighbor values DIAdem includes when approximating the interpolation points, for Akima subsplines.<div id="exp_AkimaRange">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>2 &lt;= AkimaRange &lt;= 5</td></tr>
</table>
<p class="Body">If the number of neighbor values is high, the influence of an outlier on the resulting values is low. The neighbor values then also influence the correct values.</p>
</div></td></tr>
<tr><td width="150">AkimaCoeff</td>
<td>Specifies the influence of the neighboring interpolation points when DIAdem approximates the interpolation points, for Akima subsplines.<div id="exp_AkimaCoeff">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= AkimaCoeff &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">AkimaCoeff</span> variable specifies to which extent neighboring interpolation points, which are farther away, impact the regression calculation. If you enter <span class="Monospace">1</span>, the influence of the neighboring interpolation points decreases linear.</p>
<p class="Body">If you enter <span class="Monospace">3</span> for the interpolation points and select <span class="Monospace">1</span> as the weighting factor, the actual value influences the calculation value most and the 3 neighboring interpolation points have no influence. The influence of the neighbor interpolation points decreases linearly (<span class="Monospace">1,2/3,1/3,0</span>).</p>
<p class="Body">If you select <span class="Monospace">2</span> as the weighting factor, the influence is inverse quadratic and as the interpolation points recede their influence decreases.</p>
<p class="Body">Use values from <span class="Monospace">0.5</span> to  <span class="Monospace">2.0</span>. A <span class="Monospace">0</span> weighting factor does not mean a balance, it only means that the actual value is used for the calculation.</p>
</div></td></tr>
<tr><td width="150">AkimaPerc</td>
<td>Specifies the tolerance percentage by which an approximated interpolation point may deviate from the original interpolation point, for Akima subsplines.<div id="exp_AkimaPerc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= AkimaPerc &lt;= 100</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  If you assign the value zero to the <span class="Monospace">AkimaPerc</span> variable, DIAdem does not limit the interpolation points.</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnAkimaYCalc.htm`*

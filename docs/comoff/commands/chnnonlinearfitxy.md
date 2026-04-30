---
title: "ChnNonLinearFitXY"
description: "Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non"
---

# ChnNonLinearFitXY

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNonLinearFitXY

Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non-linear function of the y = f(x,a) type. If required, DIAdem also generates the interpolation points channel necessary for the calculation.

## Signature

```python
dd.ChnNonLinearFitXY( XW , Y , ResultChannel , ResultChannel , XChnStyle, XNo, XDiv, NonLinearFitMaxIterations, NonLinearFitCovariance)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem stores the calculated coefficients and the mean squared error in the following custom properties of the result channels: <span class="Monospace">Result~NonLinearFit~Coefficient</span>, <span class="Monospace">Result~NonLinearFit~CoefficientName</span>, <span class="Monospace">Result~NonLinearFit~ModelFunction</span>, and <span class="Monospace">Result~NonLinearFit~MSE</span>. DIAdem adds to the custom properties <span class="Monospace">Result~NonLinearFit~Coefficient</span> and <span class="Monospace">Result~NonLinearFit~CoefficientName</span> a number corresponding to the number of the coefficient.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the interpolation points of the approximation function. </td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the approximation function.</td></tr>
<tr><td width="150">XChnStyle</td>
<td>Specifies which method DIAdem uses to generate the interpolation point channel.<div id="exp_XChnStyle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Partition complete area"</pre></donottranslate></td>
<td>Divide entire area</td></tr>
<tr><td width="150"><donottranslate><pre>"Partition intervals"</pre></donottranslate></td>
<td>Divide intervals</td></tr>
<tr><td width="150"><donottranslate><pre>"Use channel"</pre></donottranslate></td>
<td>Use channel</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">XNo</td>
<td>Specifies the number of values in a new data channel.<div id="exp_XNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>2 &lt;= XNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
</div></td></tr>
<tr><td width="150">XDiv</td>
<td>Specifies the number of equidistant sections in each interval of the x-range.<div id="exp_XDiv">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= XDiv &lt;= 100</td></tr>
</table>
</div></td></tr>
<tr><td width="150">NonLinearFitMaxIterations</td>
<td>Specifies the maximum number of the fitting routine iterations of a non-linear curve fitting. If the number of iterations exceeds this value, the fitting process stops.<div id="exp_NonLinearFitMaxIterations">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= NonLinearFitMaxIterations &lt;= 1000</td></tr>
</table>
</div></td></tr>
<tr><td width="150">NonLinearFitCovariance</td>
<td>Specifies whether DIAdem generates the covariance matrix for a non-linear curve fitting.<div id="exp_NonLinearFitCovariance">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table18"><tr><td width="150">NonLinearFitCoef(i)</td><td>Receives the coefficients of a non-linear curve fitting setup function.<div id="exp_NonLinearFitCoef">
<table class="Borderless" id="table19">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a><br attr="ext"/>i = 1 ... 20</td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr><tr><td width="150">NonLinearFitMSE</td><td>Receives the mean squared error of a non-linear curve fitting.<div id="exp_NonLinearFitMSE">
<table class="Borderless" id="table20">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr></table>
</div>

---

*Source: `ComOff/ChnNonLinearFitXY.htm`*

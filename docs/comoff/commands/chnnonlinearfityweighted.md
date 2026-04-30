---
title: "ChnNonLinearFitYWeighted"
description: "Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non"
---

# ChnNonLinearFitYWeighted

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNonLinearFitYWeighted

Uses the Levenberg-Marquardt algorithm to specify the least squares of the coefficients a , which best fit the input pairs, which means they also best fit a non-linear function of the y = f(x,a) type. If required, DIAdem also generates the interpolation points channel necessary for the calculation. DIAdem includes the y-channel weightings.

## Signature

```python
dd.ChnNonLinearFitYWeighted( XW , Y , Y1 , SamplingPointChn, ResultChannel , NonLinearFitMaxIterations, NonLinearFitCovariance)
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
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the weightings for the y-values of the signal.</td></tr>
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
<table class="Borderless" id="table28"><tr><td width="150">NonLinearFitCoef(i)</td><td>Receives the coefficients of a non-linear curve fitting setup function.<div id="exp_NonLinearFitCoef">
<table class="Borderless" id="table29">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a><br attr="ext"/>i = 1 ... 20</td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr><tr><td width="150">NonLinearFitMSE</td><td>Receives the mean squared error of a non-linear curve fitting.<div id="exp_NonLinearFitMSE">
<table class="Borderless" id="table30">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr></table>
</div>

---

*Source: `ComOff/ChnNonLinearFitYWeighted.htm`*

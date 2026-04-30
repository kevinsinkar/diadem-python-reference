---
title: "ChnGenLSFit"
description: "Specifies the k-dimensional linear curve values and the k-dimensional coefficients for linear fitting that best fit a k-dimensional curve using the least square"
---

# ChnGenLSFit

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnGenLSFit

Specifies the k-dimensional linear curve values and the k-dimensional coefficients for linear fitting that best fit a k-dimensional curve using the least square method.

## Signature

```python
dd.ChnGenLSFit( Y , ChnList, ResultChannel , GenLSFitCovariance, GenLSFitAlgorithm)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>DIAdem saves the mean squared error in the following custom properties of the result channels: <span class="Monospace">Result~GeneralLSLinearFit~MSE</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or <a href="../../../inavidata/collections/elementlist/">Channel list </a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the approximation function.</td></tr>
<tr><td width="150">GenLSFitCovariance</td>
<td>Specifies whether DIAdem generates the covariance matrix for a general LS linear fitting.<div id="exp_GenLSFitCovariance">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">GenLSFitAlgorithm</td>
<td>Specifies the algorithm for the general LS linear fitting.<div id="exp_GenLSFitAlgorithm">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"SVD"</pre></donottranslate></td>
<td>SVD</td></tr>
<tr><td width="150"><donottranslate><pre>"Givens"</pre></donottranslate></td>
<td>Givens</td></tr>
<tr><td width="150"><donottranslate><pre>"Givens2"</pre></donottranslate></td>
<td>Givens2</td></tr>
<tr><td width="150"><donottranslate><pre>"Householder"</pre></donottranslate></td>
<td>Householder</td></tr>
<tr><td width="150"><donottranslate><pre>"LU Decomposition"</pre></donottranslate></td>
<td>LU decomposition (triangular decomposition)</td></tr>
<tr><td width="150"><donottranslate><pre>"Cholesky"</pre></donottranslate></td>
<td>Cholesky</td></tr>
<tr><td width="150"><donottranslate><pre>"SVD for Rank Deficient H"</pre></donottranslate></td>
<td>SVD for rank deficient matrix H</td></tr>
</table>
</td></tr>
</table>The LU decomposition is also called triangular decomposition.<p>
</p></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table6"><tr><td width="150">GenLSFitMSE</td><td>Receives the mean squared error of a general LS linear fitting.<div id="exp_GenLSFitMSE">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr></table>
</div>

---

*Source: `ComOff/ChnGenLSFit.htm`*

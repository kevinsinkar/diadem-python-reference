---
title: "ChnRegrXYCalc"
description: "Uses a regression function to approximate a signal. If required, DIAdem also generates the interpolation points channel necessary for calculating the regression"
---

# ChnRegrXYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRegrXYCalc

Uses a regression function to approximate a signal. If required, DIAdem also generates the interpolation points channel necessary for calculating the regression.

## Signature

```python
return_value = dd.ChnRegrXYCalc( XW , Y , ResultChannel , ResultChannel , RegrType, XChnStyle, XNo, XDiv)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The y-channel you want to evaluate must not contain negative values when DIAdem uses a logarithmic setup function.<br attr="ext"/>Note  In addition, DIAdem saves the calculation results in the following custom properties of the result channel:  <span class="Monospace">Result~Regression~CoefficientA</span>, <span class="Monospace">Result~Regression~CoefficientB</span>, <span class="Monospace">Result~Regression~Name</span> and <span class="Monospace">Result~Regression~Precision</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the interpolation points of the regression function.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the regression function.</td></tr>
<tr><td width="150">RegrType</td>
<td>Specifies the setup function for a regression.<div id="exp_RegrType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"linear"</pre></donottranslate></td>
<td>Linear</td></tr>
<tr><td width="150"><donottranslate><pre>"power"</pre></donottranslate></td>
<td>Power</td></tr>
<tr><td width="150"><donottranslate><pre>"exponential"</pre></donottranslate></td>
<td>Exponential</td></tr>
<tr><td width="150"><donottranslate><pre>"logarith.10"</pre></donottranslate></td>
<td>Decadic logarithm</td></tr>
<tr><td width="150"><donottranslate><pre>"logarith.n"</pre></donottranslate></td>
<td>Natural logarithm</td></tr>
<tr><td width="150"><donottranslate><pre>"power no weight adjustment"</pre></donottranslate></td>
<td>Power (without weight adjustment)</td></tr>
<tr><td width="150"><donottranslate><pre>"exponential no weight adjustment"</pre></donottranslate></td>
<td>Exponential (without weight adjustment)</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
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
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnRegrXYCalc.htm`*

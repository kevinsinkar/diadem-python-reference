---
title: "ChnSplineXYCalc"
description: "Uses a non-parametrical spline to approximate a signal. If required, DIAdem also generates the interpolation points channel necessary for calculating the spline"
---

# ChnSplineXYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSplineXYCalc

Uses a non-parametrical spline to approximate a signal. If required, DIAdem also generates the interpolation points channel necessary for calculating the splines.

## Signature

```python
return_value = dd.ChnSplineXYCalc( XW , Y , ResultChannel , ResultChannel , SplineType, XChnStyle, SplineXNo, SplineXDiv, SplineWeight)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>With approximating splines, the value range is: 0 &lt;= SplineWeight &lt;= +1E300</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The values in the x-channel must be strictly monotonic increasing.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>To calculate a non-parametrical, periodic spline the first value of the y-channel must be the same as the last value.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the interpolation points of the spline function.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the y-values of the spline function.</td></tr>
<tr><td width="150">SplineType</td>
<td>Specifies the function setup for the spline function.<div id="exp_SplineType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"natural"</pre></donottranslate></td>
<td>Natural</td></tr>
<tr><td width="150"><donottranslate><pre>"approximating"</pre></donottranslate></td>
<td>Approximating</td></tr>
<tr><td width="150"><donottranslate><pre>"periodic"</pre></donottranslate></td>
<td>Periodic</td></tr>
<tr><td width="150"><donottranslate><pre>"rational"</pre></donottranslate></td>
<td>Rational</td></tr>
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
<tr><td width="150">SplineXNo</td>
<td>Specifies the number of partitions in the entire x-range.<div id="exp_SplineXNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>2 &lt;= SplineXNo &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a></td></tr>
</table>
<p class="Body">For non-parametric splines or for Akima subsplines the partitions are equidistant.</p>
</div></td></tr>
<tr><td width="150">SplineXDiv</td>
<td>Specifies the number of partitions in each interval of the x-range.<div id="exp_SplineXDiv">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= SplineXDiv &lt;= 100</td></tr>
</table>
<p class="Body">For non-parametric splines or for Akima subsplines the partitions are equidistant.</p>
</div></td></tr>
<tr><td width="150">SplineWeight</td>
<td>Specifies the weighting factor that affects the overshoot behavior in approximating splines and rational splines.<div id="exp_SplineWeight">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>-1 &lt;= SplineWeight &lt;= +1E300</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>With approximating splines, the value range is: 0 &lt;= SplineWeight &lt;= +1E300</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnSplineXYCalc("Grp/Chn1","Grp/Chn2","Grp/Chn3","Grp/Chn4","natural","Partition complete area",250,1,0)
```

---

*Source: `ComOff/ChnSplineXYCalc.htm`*

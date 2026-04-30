---
title: "ChnSplineYCalc"
description: "Uses a non-parametrical spline to approximate a signal."
---

# ChnSplineYCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSplineYCalc

Uses a non-parametrical spline to approximate a signal.

## Signature

```python
return_value = dd.ChnSplineYCalc( XW , Y , SamplingPointChn, ResultChannel , SplineType, SplineWeight)
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
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
dd.ChnSplineYCalc("Grp/Chn1","Grp/Chn2","Grp/Chn3","Grp/Chn4","natural",0)
```

---

*Source: `ComOff/ChnSplineYCalc.htm`*

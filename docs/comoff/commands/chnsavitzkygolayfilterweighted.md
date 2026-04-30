---
title: "ChnSavitzkyGolayFilterWeighted"
description: "Uses weighting factors to smooth a data channel with the Savitzky-Golay filter."
---

# ChnSavitzkyGolayFilterWeighted

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSavitzkyGolayFilterWeighted

Uses weighting factors to smooth a data channel with the Savitzky-Golay filter.

## Signature

```python
return_value = dd.ChnSavitzkyGolayFilterWeighted( Y , Y1 , ResultChannel , PolynomialOrder, SmoothWidth)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel with the weighting for the minimization of the least squares. The channel must have a minimum length of <span class="Monospace">2 * <a href="../../../varoff/variables/smoothwidth/">SmoothWidth</a> + 1</span>.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">PolynomialOrder</td>
<td>Specifies the order of the polynomial.<div id="exp_PolynomialOrder">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= PolynomialOrder &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">SmoothWidth</td>
<td>Specifies the number of neighboring values to the left and right of the channel value that DIAdem uses to calculate the mean.<div id="exp_SmoothWidth">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger</a></td></tr>
<tr>
<td>1 &lt;= SmoothWidth &lt;= <a href="../../../varoff/variables/globchnlength/">GlobChnLength</a><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnSavitzkyGolayFilterWeighted.htm`*

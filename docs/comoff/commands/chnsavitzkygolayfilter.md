---
title: "ChnSavitzkyGolayFilter"
description: "Smoothes a data channel with the Savitzky-Golay filter."
---

# ChnSavitzkyGolayFilter

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSavitzkyGolayFilter

Smoothes a data channel with the Savitzky-Golay filter.

## Signature

```python
return_value = dd.ChnSavitzkyGolayFilter( Y , ResultChannel , PolynomialOrder, SmoothWidth)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
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

*Source: `ComOff/ChnSavitzkyGolayFilter.htm`*

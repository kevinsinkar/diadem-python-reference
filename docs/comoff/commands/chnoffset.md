---
title: "ChnOffset"
description: "Subtracts an offset from the channel values or adds an offset to the channel values."
---

# ChnOffset

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnOffset

Subtracts an offset from the channel values or adds an offset to the channel values.

## Signature

```python
return_value = dd.ChnOffset( Y , ResultChannel , ChnOffsetValue, ChnOffsetMode)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">ChnOffsetValue</td>
<td>Specifies the number of values that DIAdem averages or the free offset that DIAdem adds to the individual channel values.<div id="exp_ChnOffsetValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ChnOffsetMode</td>
<td>Specifies the type of offset correction DIAdem uses.<div id="exp_ChnOffsetMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"free offset"</pre></donottranslate></td>
<td>Add any offset</td></tr>
<tr><td width="150"><donottranslate><pre>"first value offset"</pre></donottranslate></td>
<td>Subtracting first channel value</td></tr>
<tr><td width="150"><donottranslate><pre>"min. value offset"</pre></donottranslate></td>
<td>Subtracting minimum channel value</td></tr>
<tr><td width="150"><donottranslate><pre>"last value offset"</pre></donottranslate></td>
<td>Subtracting last channel value</td></tr>
<tr><td width="150"><donottranslate><pre>"max. value offset"</pre></donottranslate></td>
<td>Subtracting maximum channel value</td></tr>
<tr><td width="150"><donottranslate><pre>"mean value offset"</pre></donottranslate></td>
<td>Subtracting average of the first n values</td></tr>
</table>
</td></tr>
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

*Source: `ComOff/ChnOffset.htm`*

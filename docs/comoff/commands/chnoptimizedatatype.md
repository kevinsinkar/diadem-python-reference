---
title: "ChnOptimizeDataType"
description: "Optimizes the data type of a channel to save disk space."
---

# ChnOptimizeDataType

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnOptimizeDataType

Optimizes the data type of a channel to save disk space.

## Signature

```python
return_value = dd.ChnOptimizeDataType( X , OptimizeDataTypeRoundMode, OptimizeDataTypeRoundDigitType, OptimizeDataTypeRoundDigitCount, OptimizeDataTypeIP)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150">OptimizeDataTypeRoundMode</td>
<td>Specifies the rounding mode for data optimization.<div id="exp_OptimizeDataTypeRoundMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Standard"</pre></donottranslate></td>
<td>Round mathematically</td></tr>
<tr><td width="150"><donottranslate><pre>"Truncate"</pre></donottranslate></td>
<td>Truncating</td></tr>
<tr><td width="150"><donottranslate><pre>"RoundDown"</pre></donottranslate></td>
<td>Round down</td></tr>
<tr><td width="150"><donottranslate><pre>"RoundUp"</pre></donottranslate></td>
<td>Round up</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OptimizeDataTypeRoundDigitType</td>
<td>Specifies which places DIAdem rounds in order to optimize the data.<div id="exp_OptimizeDataTypeRoundDigitType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>Automatic</td></tr>
<tr><td width="150"><donottranslate><pre>"DecimalDigits"</pre></donottranslate></td>
<td>Round to n decimal places</td></tr>
<tr><td width="150"><donottranslate><pre>"FirstDigits"</pre></donottranslate></td>
<td>Round to n places</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OptimizeDataTypeRoundDigitCount</td>
<td>Specifies how many places DIAdem rounds in order to optimize the data.<div id="exp_OptimizeDataTypeRoundDigitCount">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= OptimizeDataTypeRoundDigitCount &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OptimizeDataTypeIP</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result channels of the data optimization.<div id="exp_OptimizeDataTypeIP">
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
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnOptimizeDataType.htm`*

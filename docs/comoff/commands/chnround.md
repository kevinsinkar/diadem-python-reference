---
title: "ChnRound"
description: "Rounds a channel."
---

# ChnRound

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnRound

Rounds a channel.

## Signature

```python
return_value = dd.ChnRound( X , RoundMode, RoundDigitType, RoundDigitCount, RoundIP)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150">RoundMode</td>
<td>Specifies the rounding mode.<div id="exp_RoundMode">
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
<tr><td width="150">RoundDigitType</td>
<td>Specifies which places DIAdem rounds.<div id="exp_RoundDigitType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Automatic"</pre></donottranslate></td>
<td>DIAdem rounds to the last significant place</td></tr>
<tr><td width="150"><donottranslate><pre>"DecimalDigits"</pre></donottranslate></td>
<td>Round to n decimal places</td></tr>
<tr><td width="150"><donottranslate><pre>"FirstDigits"</pre></donottranslate></td>
<td>Round to n places</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RoundDigitCount</td>
<td>Specifies how many places DIAdem rounds.<div id="exp_RoundDigitCount">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= RoundDigitCount &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">RoundIP</td>
<td>Specifies whether DIAdem overwrites the values of the input channels with the result channels when rounding.<div id="exp_RoundIP">
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

*Source: `ComOff/ChnRound.htm`*

---
title: "ChnACDCCoupling"
description: "Removes the bias (DAC part) from a signal. DIAdem uses an FFT window function before summating all signal values in order to specify the bias of the signal. DIA"
---

# ChnACDCCoupling

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnACDCCoupling

Removes the bias (DAC part) from a signal. DIAdem uses an FFT window function before summating all signal values in order to specify the bias of the signal. DIAdem then subtracts this one value from each value of the input signal.

## Signature

```python
return_value = dd.ChnACDCCoupling( Y , ResultChannel , ACDCWndFct)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel from which DIAdem removes the bias.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">ACDCWndFct</td>
<td>Specifies which window function DIAdem uses on the entire input channel.<div id="exp_ACDCWndFct">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Rectangle"</pre></donottranslate></td>
<td>Rectangle</td></tr>
<tr><td width="150"><donottranslate><pre>"Hanning"</pre></donottranslate></td>
<td>Hanning</td></tr>
<tr><td width="150"><donottranslate><pre>"Hamming"</pre></donottranslate></td>
<td>Hamming</td></tr>
<tr><td width="150"><donottranslate><pre>"Blackman"</pre></donottranslate></td>
<td>Blackman</td></tr>
<tr><td width="150"><donottranslate><pre>"FlatTop"</pre></donottranslate></td>
<td>FlatTop</td></tr>
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

*Source: `ComOff/ChnACDCCoupling.htm`*

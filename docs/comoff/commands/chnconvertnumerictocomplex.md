---
title: "ChnConvertNumericToComplex"
description: "Generates a complex channel from a numeric channel pair."
---

# ChnConvertNumericToComplex

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertNumericToComplex

Generates a complex channel from a numeric channel pair.

## Signature

```python
return_value = dd.ChnConvertNumericToComplex( Y1 , Y2 , ChnPairMode )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong> Complex channels are a preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the real part or magnitude values.</td></tr>
<tr><td width="150"><em>Y2</em></td>
<td>Specifies the data channel containing the imaginary part or phase values.</td></tr>
<tr><td width="150">ChnPairMode</td>
<td>Specifies whether the numeric channel pair is real and imaginary part or magnitude and phase. In <a href="#" data-unresolved="1">non-quantity-based calculations</a>, DIAdem expects the phase in <span class="Monospace">rad</span>.<div id="exp_ChnPairMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"cartesian"</pre></donottranslate></td>
<td>Real and imaginary part</td></tr>
<tr><td width="150"><donottranslate><pre>"polar"</pre></donottranslate></td>
<td>Magnitude and phase</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the complex result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertNumericToComplex.htm`*

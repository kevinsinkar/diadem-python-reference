---
title: "ChnConvertComplexToNumeric"
description: "Creates a numeric channel pair from a complex channel."
---

# ChnConvertComplexToNumeric

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertComplexToNumeric

Creates a numeric channel pair from a complex channel.

## Signature

```python
return_value = dd.ChnConvertComplexToNumeric( Y , ChnPairMode )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note</strong> Complex channels are a preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel with the complex values.</td></tr>
<tr><td width="150">ChnPairMode</td>
<td>Specifies whether the numeric channel pair is real and imaginary part or magnitude and phase.<div id="exp_ChnPairMode">
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
<td>Contains the numeric channel pair with the real and the imaginary part or the magnitude and phase in <span class="Monospace">rad</span>. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertComplexToNumeric.htm`*

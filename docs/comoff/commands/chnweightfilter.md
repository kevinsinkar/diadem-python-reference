---
title: "ChnWeightFilter"
description: "Executes a frequency weighted digital filter."
---

# ChnWeightFilter

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnWeightFilter

Executes a frequency weighted digital filter.

## Signature

```python
return_value = dd.ChnWeightFilter( XW , Y , ResultChannel , WeightFilterType, [SoundLevelTimeWeighting], [SoundLevelResultInDb])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the x-values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values of the signal.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">WeightFilterType</td>
<td>Specifies the frequency weighted curve of the digital filter.<div id="exp_WeightFilterType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"AWeight"</pre></donottranslate></td>
<td>A weighting</td></tr>
<tr><td width="150"><donottranslate><pre>"BWeight"</pre></donottranslate></td>
<td>B weighting</td></tr>
<tr><td width="150"><donottranslate><pre>"CWeight"</pre></donottranslate></td>
<td>C weighting</td></tr>
</table>
</td></tr>
</table>The A evaluation corresponds with curves of the same volume level at 20-40 phon, the B evaluation corresponds with the volume level at 50-70 phon, and the C evaluation corresponds with the volume level at 80-90 phon.</div></td></tr>
<tr><td width="150">[SoundLevelTimeWeighting]</td>
<td>Determines the time constant for the time weighting of a sound level.<div id="exp_SoundLevelTimeWeighting">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"none"</pre></donottranslate></td>
<td>None</td></tr>
<tr><td width="150"><donottranslate><pre>"slow"</pre></donottranslate></td>
<td>Slow</td></tr>
<tr><td width="150"><donottranslate><pre>"fast"</pre></donottranslate></td>
<td>Fast</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[SoundLevelResultInDb]</td>
<td>Determines, whether the result of the ABC filtering is output in dB.<div id="exp_SoundLevelResultInDb">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnWeightFilter.htm`*

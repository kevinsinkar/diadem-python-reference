---
title: "ChnSoundLevelAverage"
description: "Calculation of a time-weighted sound level"
---

# ChnSoundLevelAverage

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnSoundLevelAverage

Calculation of a time-weighted sound level

## Signature

```python
return_value = dd.ChnSoundLevelAverage( XW , Y , SoundLevelTimeWeighting, SoundLevelResultType, [SoundLevelReferenceValue])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the xw-values. If all associated y-channels are waveform channels and you do not specify the xw-channel, DIAdem uses the x-part of the associated waveform channels.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">SoundLevelTimeWeighting</td>
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
<tr><td width="150">SoundLevelResultType</td>
<td>Determines the form in which the result of the sound level calculation is output.<div id="exp_SoundLevelResultType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"power"</pre></donottranslate></td>
<td>power</td></tr>
<tr><td width="150"><donottranslate><pre>"amplitude"</pre></donottranslate></td>
<td>Amplitude</td></tr>
<tr><td width="150"><donottranslate><pre>"dB"</pre></donottranslate></td>
<td>dB</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[SoundLevelReferenceValue]</td>
<td>Determines the reference value for the dB calculation of a sound level.<div id="exp_SoundLevelReferenceValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number</a></td></tr>
<tr>
<td>0.0 &lt;= SoundLevelReferenceValue &lt;= 1E30<br attr="ext"/>Access: Read/Write</td></tr>
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

*Source: `ComOff/ChnSoundLevelAverage.htm`*

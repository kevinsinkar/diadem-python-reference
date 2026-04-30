---
title: "ChnConvertNumericToWaveform"
description: "Valid names: ChnConvertNumericToWaveform, ChnToWfChn"
---

# ChnConvertNumericToWaveform

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertNumericToWaveform

Valid names: ChnConvertNumericToWaveform, ChnToWfChn

## Signature

```python
dd.ChnConvertNumericToWaveform( X , ChnList, [XChnDelete], [WfXStartTimeMode])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>X</em></td>
<td>Specifies the data channel containing the x-values.</td></tr>
<tr><td width="150">ChnList</td>
<td>Specifies one or more channels.<div id="exp_ChnList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
</tr>
</table>
<p>A channel list is a <a href="../../../inavidata/objects/idiademchannel/">Channel</a> or a <a href="../../../inavidata/collections/elementlist/">Channel list</a> object, or a text that refers to one or several channels. For more information about the value range, refer to <a href="#" data-unresolved="1">Channel lists</a>.</p>
</div></td></tr>
<tr><td width="150">[XChnDelete]</td>
<td>Specifies whether DIAdem deletes the x-channel after the operation. The default value is <span class="Monospace">FALSE</span> which means that DIAdem does not delete the x-channel.<div id="exp_XChnDelete">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[WfXStartTimeMode]</td>
<td>Specifies the type of time reference when converting numeric channels to waveform channels, and whether DIAdem considers the waveform start time when converting waveform channels to numeric channels or when generating a channel from the x-part of a waveform channel.<div id="exp_WfXStartTimeMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"WfXRelative"</pre></donottranslate></td>
<td>Relative time reference</td></tr>
<tr><td width="150"><donottranslate><pre>"WfXAbsolute"</pre></donottranslate></td>
<td>Absolute time reference</td></tr>
</table>
</td></tr>
</table>If you convert numeric channels to waveform channels, the <span class="Monospace">WfXStartTimeMode</span> variable specifies whether DIAdem generates waveforms with relative or absolute time reference. For absolute time reference, the x-channel must be a DIAdem time channel. If you convert waveform channels to numeric channels, the <span class="Monospace">WfXStartTimeMode</span> variable specifies whether DIAdem considers the waveform start time. If you consider the start time (absolute time reference), DIAdem generates a time channel, otherwise DIAdem generates a numeric channel (relative time reference).</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertNumericToWaveform.htm`*

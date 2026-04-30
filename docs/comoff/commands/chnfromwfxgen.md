---
title: "ChnFromWfXGen"
description: "Generates a data channel from the x-part of a specified waveform channel."
---

# ChnFromWfXGen

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnFromWfXGen

Generates a data channel from the x-part of a specified waveform channel.

## Signature

```python
return_value = dd.ChnFromWfXGen( Y , ResultChannel , [WfXStartTimeMode])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the waveform channel which has the x-parts that provide the x-values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
<tr><td width="150">[WfXStartTimeMode]</td>
<td>Specifies the type of time reference when converting numeric channels to waveform channels, and whether DIAdem considers the waveform start time when converting waveform channels to numeric channels or when generating a channel from the x-part of a waveform channel. <div id="exp_WfXStartTimeMode">
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

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnFromWfXGen.htm`*

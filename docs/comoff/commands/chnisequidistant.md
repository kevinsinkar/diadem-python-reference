---
title: "ChnIsEquidistant"
description: "Specifies whether a channel is equidistant."
---

# ChnIsEquidistant

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnIsEquidistant

Specifies whether a channel is equidistant.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the y-values.</td></tr>
<tr><td width="150">FullValueEquidistantCheck</td>
<td>Specifies if DIAdem checks whether all values are equidistant or if only a sample is equidistant.<div id="exp_FullValueEquidistantCheck">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">EquidistantCheckMode</td>
<td>Specifies whether DIAdem checks all channels or only strictly monotonic channels.<div id="exp_EquidistantCheckMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"CheckAll"</pre></donottranslate></td>
<td>Check always</td></tr>
<tr><td width="150"><donottranslate><pre>"CheckDecreasing"</pre></donottranslate></td>
<td>Check monotonic falling channels</td></tr>
<tr><td width="150"><donottranslate><pre>"CheckIncreasing"</pre></donottranslate></td>
<td>Check monotonic increasing channels</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean variable</a> type. The return value is <span class="Monospace">True</span> when the channel is equidistant and the values correspond to the monotony defined in the <span class="Monospace">EquidistantCheckMode</span> variable. Otherwise the return value is <span class="Monospace">False</span>.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnIsEquidistant.htm`*

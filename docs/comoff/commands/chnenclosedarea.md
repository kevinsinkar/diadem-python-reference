---
title: "ChnEnclosedArea"
description: "Calculates the area between two or more curves or one curve and the x-axis."
---

# ChnEnclosedArea

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnEnclosedArea

Calculates the area between two or more curves or one curve and the x-axis.

## Signature

```python
return_value = dd.ChnEnclosedArea([ XChannels ], YChannels , [AreaLimitMode], [AreaSummationMode], ResultChannel , ResultChannel , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">[XChannels]</td>
<td>Specifies the x-channels of the curves.<div id="exp_XChannels">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
<p class="Body">For waveform channels, you do not need to specify x-channels.</p>
</div></td></tr>
<tr><td width="150">YChannels</td>
<td>Specifies the y-channels of the curves. <div id="exp_YChannels">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Channel list variable</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
<tr><td width="150">[AreaLimitMode]</td>
<td>Specifies the x-value range of the area calculation.<div id="exp_AreaLimitMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"AllOverlap"</pre></donottranslate></td>
<td>Joint x-value range of all curves</td></tr>
<tr><td width="150"><donottranslate><pre>"MinOverlap"</pre></donottranslate></td>
<td>Joint x-value range of at least two curves</td></tr>
</table>
</td></tr>
</table>
<h2>Valid Settings</h2>
<table class="Borderless">
<tr>
<td><donottranslate><pre>"AllOverlap"</pre></donottranslate></td>
<td>DIAdem calculates the area through the length on which the x-value ranges of all curves overlap.</td>
</tr>
<tr>
<td><donottranslate><pre>"MinOverlap"</pre></donottranslate></td>
<td>DIAdem calculates the area over the length on which the x-value ranges of at least two curves overlap.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[AreaSummationMode]</td>
<td>Determines whether the area calculation includes signs when adding the partial areas.<div id="exp_AreaSummationMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"Absolute"</pre></donottranslate></td>
<td>Amounts of the partial areas</td></tr>
<tr><td width="150"><donottranslate><pre>"Signed"</pre></donottranslate></td>
<td>Partial area with sign</td></tr>
</table>
</td></tr>
</table>
<h2>Valid Settings</h2>
<p class="Body">DIAdem evaluates this variable only for one curve or two curves. For more than two curves, DIAdem adds the sums of the partial areas.</p>
<table class="Borderless">
<tr>
<td><donottranslate><pre>"Absolute"</pre></donottranslate></td>
<td>DIAdem adds the amounts of the partial areas regardless of the position of the partial areas to the first curve or the x-axis.</td>
</tr>
<tr>
<td><donottranslate><pre>"Signed"</pre></donottranslate></td>
<td>DIAdem adds the partial areas with signs. DIAdem assigns a negative sign to a partial area if the partial area is below the first curve. If the command <span class="Monospace">ChnEnclosedArea</span> calculates the area between only one curve and the x-axis, the partial areas below the x-axis receive negative signs.</td>
</tr>
</table>
</div></td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel containing the x-values of the partial areas.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel with the partial areas.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel with the summated partial areas.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

## Python example

```python
oMyXChns = dd.Data.GetChannels("[1]/Time*")
oMyYChns = dd.Data.GetChannels("[1]/Speed*")
oMyResultChn = dd.ChnEnclosedArea(oMyXChns,oMyYChns, "AllOverlap", "Absolute", "[1]/Segments", "[1]/Areas", "[1]/SumOfAreas")
dd.MsgboxDisp("First result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name)
```

```python
oMyResultChn= dd.ChnEnclosedArea("","'[2]/Noise_1','[2]/Noise_2'","AllOverlap","Signed", "/Segments", "/Areas", "/SumOfAreas")
dd.MsgboxDisp("First result channel: " + oMyResultChn(1).ChannelGroup.Name + "/" + oMyResultChn(1).Name)
```

---

*Source: `ComOff/ChnEnclosedArea.htm`*

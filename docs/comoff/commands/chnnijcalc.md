---
title: "ChnNijCalc"
description: "Calculates the Normalized Neck Injury Criterion value (Nij) according to FMVSS."
---

# ChnNijCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNijCalc

Calculates the Normalized Neck Injury Criterion value (Nij) according to FMVSS.

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem saves the calculation results and the version number of the algorithm used, which is not the same as the DIAdem version number, in the following custom properties of the result channels <span class="Monospace">LoadConditionNTF</span>, <span class="Monospace">LoadConditionNTE</span>, <span class="Monospace">LoadConditionNCE</span>, and <span class="Monospace">LoadConditionNCF</span>: <span class="Monospace">Result~Nij~Max</span>, <span class="Monospace">Result~Nij~Time</span>, <span class="Monospace">Result~Nij~Type</span>, and <span class="Monospace">Result~Nij~Version</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">NIJ criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values in milliseconds. The values of the data channel must be monotonic increasing. If the y-channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the values of the axial force in the z-direction at the point where the head intersects with the neck, in Newton.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the values of the bending moment (total moment) in the y-direction at the top of the neck, in newton meters.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the NIC evaluation curve.</td></tr>
<tr><td width="150">NijFzc</td>
<td>Specifies the critical compression force in newtons.<div id="exp_NijFzc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">NijMyc</td>
<td>Specifies the critical bending moment in newton meters.<div id="exp_NijMyc">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">NijType</td>
<td>Specifies the calculation type.<div id="exp_NijType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"NTE"</pre></donottranslate></td>
<td>NTE</td></tr>
<tr><td width="150"><donottranslate><pre>"NTF"</pre></donottranslate></td>
<td>NTF</td></tr>
<tr><td width="150"><donottranslate><pre>"NCE"</pre></donottranslate></td>
<td>NCE</td></tr>
<tr><td width="150"><donottranslate><pre>"NCF"</pre></donottranslate></td>
<td>NCF</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the version number of the NIJ calculation routine. The return value is an NIJVersion type.<div id="exp_NIJVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnNijCalc.htm`*

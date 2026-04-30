---
title: "ChnACompCalc"
description: "Calculates the average acceleration during the compression phase."
---

# ChnACompCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnACompCalc

Calculates the average acceleration during the compression phase.

## Signature

```python
dd.ChnACompCalc( XW , Y , ACompStartTime, ACompTangentType, ACompSpeed0, ACompSpeedFactor)
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  In addition, DIAdem saves the calculated results and the version number, which is independent of the DIAdem version, in the following custom properties of the input channel: <span class="Monospace">ResultACompAverage</span>, <span class="Monospace">ResultACompEndTime</span>, and <span class="Monospace">ResultACompVersion</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">AComp-criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the unfiltered acceleration values.</td></tr>
<tr><td width="150">ACompStartTime</td>
<td>Specifies the start time for the AComp calculation.<div id="exp_ACompStartTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ACompTangentType</td>
<td>Specifies the tangent type for the AComp calculation.<div id="exp_ACompTangentType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"ACompSpeed"</pre></donottranslate></td>
<td>T2 calculated from velocity</td></tr>
<tr><td width="150"><donottranslate><pre>"ACompTangent"</pre></donottranslate></td>
<td>T2 calculated from tangent</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ACompSpeed0</td>
<td>Specifies the start value of the velocity in the AComp calculation.<div id="exp_ACompSpeed0">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ACompSpeedFactor</td>
<td>Specifies the factor for the conversion of the units in the AComp calculation.<div id="exp_ACompSpeedFactor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ACompEndTime</td><td>Receives the end time for the AComp calculation.<div id="exp_ACompEndTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ACompAverage</td><td>Receives the calculated mean acceleration.<div id="exp_ACompAverage">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ACompVer</td><td>Receives the version number of the AComp calculation routine.<div id="exp_ACompVer">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnACompCalc.htm`*

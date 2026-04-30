---
title: "ChnNICRearCalc"
description: "Calculates the Neck Injury Criterion Rear Impact."
---

# ChnNICRearCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNICRearCalc

Calculates the Neck Injury Criterion Rear Impact.

## Signature

```python
return_value = dd.ChnNICRearCalc( XW , Y , Y1 , ResultChannel )
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>According to the legal stipulations, the accelerations must be filtered with CFC180.</td></tr></table>
<table class="Borderless">
<tr>
<td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  DIAdem saves the calculation results and the version number of the algorithm which is not the same as the DIAdem version number in the following custom properties of the result channel: <span class="Monospace">Result~NICRear~Max</span>, <span class="Monospace">Result~NICRear~Time</span> and <span class="Monospace">Result~NICRear~Version</span>.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">NIC (rear impact) criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel with the acceleration values of the head in the x-direction, in meters per square second.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the acceleration values of the first spinal vertebra in the x-direction, in meters per square second.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the NIC evaluation curve.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnNICRearCalc.htm`*

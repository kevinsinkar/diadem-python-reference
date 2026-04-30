---
title: "ChnLateralShoulderRibDisplacement"
description: "Calculates the Lateral Shoulder Rib Displacement value which is a criteria for the lateral shift of the shoulder ribs."
---

# ChnLateralShoulderRibDisplacement

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnLateralShoulderRibDisplacement

Calculates the Lateral Shoulder Rib Displacement value which is a criteria for the lateral shift of the shoulder ribs.

## Signature

```python
return_value = dd.ChnLateralShoulderRibDisplacement( XW , Y , Y1 , ResultChannel )
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values. If the y-channels are waveform channels, you do not need to specify this channel.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel with the IR-TRACC lengths.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel with the IR-TRACC angles.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnLateralShoulderRibDisplacement.htm`*

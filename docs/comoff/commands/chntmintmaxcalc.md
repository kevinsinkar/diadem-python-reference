---
title: "ChnTMinTMaxCalc"
description: "Determines the time points of the minimum and maximum values in a signal."
---

# ChnTMinTMaxCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnTMinTMaxCalc

Determines the time points of the minimum and maximum values in a signal.

## Signature

```python
dd.ChnTMinTMaxCalc( XW , Y )
```

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the descriptions of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel that contains the time values of the signal.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel that contains the amplitude values of the signal.</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">MinTime</td><td>Receives the time of the minimum value.<div id="exp_MinTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MaxTime</td><td>Receives the time of the maximum value.<div id="exp_MaxTime">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">MinMaxVer</td><td>Receives the version number of the MinMax calculation routine.<div id="exp_MinMaxVer">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnTMinTMaxCalc.htm`*

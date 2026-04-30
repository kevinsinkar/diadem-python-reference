---
title: "ChnTimeAreaCopy"
description: "Copies a time range and the related amplitudes into two new data channels."
---

# ChnTimeAreaCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnTimeAreaCopy

Copies a time range and the related amplitudes into two new data channels.

## Notes

<div markdown="1">
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  Refer to the descriptions of the <a href="#" data-unresolved="1">Crash Analysis Criteria</a> for further information such as background, input values, and rules and regulations.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the amplitude values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the time values.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel for the amplitudes.</td></tr>
<tr><td width="150">TimeAreaCopyBeg</td>
<td>Specifies the earlier value of the time domain.<div id="exp_TimeAreaCopyBeg">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">TimeAreaCopyEnd</td>
<td>Specifies the later value of the time domain.<div id="exp_TimeAreaCopyEnd">
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
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies the version number of the calculation routine. The return value is a TimeAreaCopyVer type.<div id="exp_TimeAreaCopyVer">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnTimeAreaCopy.htm`*

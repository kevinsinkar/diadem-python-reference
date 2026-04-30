---
title: "ChnNICBdryCalc"
description: "Calculates the Neck Injury Criterion value (NIC) according to ECE."
---

# ChnNICBdryCalc

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnNICBdryCalc

Calculates the Neck Injury Criterion value (NIC) according to ECE.

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The input channels must be filtered with CFC600.</td></tr></table>
<table class="Borderless" id="table2"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>This command adds the x and the y-values of the NIC boundary curve to the <a href="../chnniccalc/">ChnNICCalc</a> command.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The NIC calculation in DIAdem 11.0 and earlier versions is different. DIAdem now uses the cumulative calculation of all peaks according to the EuroNCAP. You can use <a href="#" data-unresolved="1">Time at Level</a> for a continuous calculation within a peak.</td></tr></table>
<table class="Borderless">
<tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the description of the <a href="#" data-unresolved="1">NIC (front impact ECE) criterion</a> for further information such as the mathematical background, input values, and directives and laws.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>XW</em></td>
<td>Specifies the data channel containing the time values in seconds.</td></tr>
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the forces in kilonewtons.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the load duration in seconds.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the amplitudes in kilonewtons.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the injury probability.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the x-values of the NIC boundary curve.</td></tr>
<tr><td width="150"><em>ResultChannel</em></td>
<td>Specifies the result channel that receives the y-values of the NIC boundary curve.</td></tr>
<tr><td width="150">NICForceType</td>
<td>Specifies whether the forces are axial tensile forces or shear forces.<div id="exp_NICForceType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Enumeration variable</a></td></tr>
<tr>
<td>Enumeration variable with the following selection terms<table class="Borderless">
<tr><td style="border-bottom-style: solid; border-bottom-width: 1" width="150"><strong>Script Term</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1"><strong>Interface Term, Explanation</strong></td></tr>
<tr><td width="150"><donottranslate><pre>"tensile force"</pre></donottranslate></td>
<td>Tensile force</td></tr>
<tr><td width="150"><donottranslate><pre>"shear force"</pre></donottranslate></td>
<td>Shear force</td></tr>
</table>
</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the version number of the FFC calculation routine. The return value is a NICVersion type.<div id="exp_NICVersion">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Word variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOff/ChnNICBdryCalc.htm`*

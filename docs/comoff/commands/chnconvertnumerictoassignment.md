---
title: "ChnConvertNumericToAssignment"
description: "Valid names: ChnConvertNumericToAssignment, ChnToAssignmentChn"
---

# ChnConvertNumericToAssignment

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertNumericToAssignment

Valid names: ChnConvertNumericToAssignment, ChnToAssignmentChn

## Signature

```python
return_value = dd.ChnConvertNumericToAssignment( Y , Y1 , DefaultValue, [DeleteAssignments])
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the numeric values. The channel must be a numeric channel, a waveform channel, or an assignment channel.<br attr="ext"/>If the first channel is an assignment channel, the existing assignment parameters are replaced with the assignment values of the second channel.</td></tr>
<tr><td width="150"><em>Y1</em></td>
<td>Specifies the data channel containing the text assignment values. The channel can be a text channel, an enumeration channel (Bus-Log-Converter), or an assignment channel.<br attr="ext"/>If the channel Y1 is an <a href="#" data-unresolved="1">Assignment channel</a>, DIAdem transfers the <a href="#" data-unresolved="1">Assignment channel parameters</a> unchanged to the new assignment channel.<br attr="ext"/>If channel Y1 is an <a href="#" data-unresolved="1">enumeration channel</a>, DIAdem generates the assignment channel parameters from the channel properties <span class="Monospace">CANEnumSubst</span> and <span class="Monospace">EnumValues</span>. Both properties must have the same number of elements for this. If the enumeration channel only contains the property <span class="Monospace">EnumValues</span>, DIAdem generates the assignments from the values of the enumeration channel and the custom properties. Therefore the enumeration channel must not contain NoValues.<br attr="ext"/>If the channel Y1 is a <a href="#" data-unresolved="1">Text channel</a>, DIAdem generates the assignments from the values of the numeric channel and from the texts of the text channel. Therefore the numeric channel must not contain NoValues.<br attr="ext"/>If you do not specify the channel Y1, DIAdem assigns an assignment channel containing the value  of <span class="Monospace">DefaultValue</span>. You can edit assignments in the dialog box <a href="#" data-unresolved="1">Assignment Parameters</a> or with a script using the property <a href="../../../inavidata/properties/idiademassignmentchannel-assignmentlist/">AssignmentList</a>.<br attr="ext"/>If you do not specify the channel Y1, DIAdem ignores the parameter <span class="Monospace">DeleteAssignments</span>.</td></tr>
<tr><td width="150">DefaultValue</td>
<td>Specifies the text which DIAdem uses in assignment channels when no text is assigned to the value.<div id="exp_DefaultValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[DeleteAssignments]</td>
<td>Specifies that DIAdem deletes the assignments for the <a href="#" data-unresolved="1">AssignmentChnToNumericChn</a> command and replaces the numeric channel with the assignment channel for the <a href="#" data-unresolved="1">ChnToAssignmentChn</a> command and also that DIAdem deletes the channel from where the assignment texts originate. The default value of the variable is <span class="Monospace">FALSE</span>.<div id="exp_DeleteAssignments">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ChnResult</em></td>
<td>Contains the result channel or result channels. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertNumericToAssignment.htm`*

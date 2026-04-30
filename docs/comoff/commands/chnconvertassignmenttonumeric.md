---
title: "ChnConvertAssignmentToNumeric"
description: "Valid names: ChnConvertAssignmentToNumeric, AssignmentChnToNumericChn"
---

# ChnConvertAssignmentToNumeric

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertAssignmentToNumeric

Valid names: ChnConvertAssignmentToNumeric, AssignmentChnToNumericChn

## Signature

```python
return_value = dd.ChnConvertAssignmentToNumeric( Y , ReplaceWithNoValue, [DeleteAssignments])
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The y-channel must be an assignment channel. DIAdem adds the numeric channel behind the assignment channel to the Data Portal and uses the channel name of the assignment channel with the extension <span class="Monospace">Numeric</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">ReplaceWithNoValue</td>
<td>Specifies that DIAdem replaces the values in the numeric channel with NoValues, which are connected to assignments in the assignment channel. The default value of the variable is <span class="Monospace">FALSE</span>, so that DIAdem does not replace the values originally connected with assignments with NoValues.<div id="exp_ReplaceWithNoValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
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
<td>Contains the result channel. <a href="../../../inavidata/collections/elementlist/">ElementList &lt;Data&gt;</a> type return value.</td></tr>
</table>
</div>

---

*Source: `ComOff/ChnConvertAssignmentToNumeric.htm`*

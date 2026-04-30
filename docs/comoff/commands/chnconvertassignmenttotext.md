---
title: "ChnConvertAssignmentToText"
description: "Valid names: ChnConvertAssignmentToText, AssignmentChnToChn"
---

# ChnConvertAssignmentToText

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertAssignmentToText

Valid names: ChnConvertAssignmentToText, AssignmentChnToChn

## Signature

```python
return_value = dd.ChnConvertAssignmentToText( Y , KeepAssignmentProperties)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The y-channel must be an assignment channel. DIAdem adds the text channel behind the assignment channel to the Data Portal and uses the channel name of the assignment channel with the extension <span class="Monospace">Text</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">KeepAssignmentProperties</td>
<td>Specifies that the assignment channel remains when DIAdem writes the assignments into a new text channel. The default value of the variable is <span class="Monospace">TRUE</span>, so that DIAdem does not delete the assignments in the assignment channel.<div id="exp_KeepAssignmentProperties">
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

*Source: `ComOff/ChnConvertAssignmentToText.htm`*

---
title: "ChnConvertTextToAssignment"
description: "Valid names: ChnConvertTextToAssignment, TextChnToAssignmentChn"
---

# ChnConvertTextToAssignment

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ChnConvertTextToAssignment

Valid names: ChnConvertTextToAssignment, TextChnToAssignmentChn

## Signature

```python
return_value = dd.ChnConvertTextToAssignment( Y , DefaultValue, DeleteTextChannel)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>The y-channel must be a text channel.<p class="body">DIAdem generates an assignment from every text in the text channel and assigns a value to every text. The first text gets the value 1 and the subsequent texts a value incremented by <span class="Monospace">1</span>. Additionally DIAdem converts the values of the assignments as channel values into the assignment channel. If a text is the same as the default value, DIAdem does not generate an assignment from this text and enters the value <span class="Monospace">0</span> for the channel value.</p>
</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150"><em>Y</em></td>
<td>Specifies the data channel containing the y-values.</td></tr>
<tr><td width="150">DefaultValue</td>
<td>Specifies the text which DIAdem uses in assignment channels when no text is assigned to the value.<div id="exp_DefaultValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">DeleteTextChannel</td>
<td>Specifies that DIAdem deletes the text channel which contains the texts for the assignments. The default value of the variable is <span class="Monospace">FALSE</span>, so that DIAdem does not delete the channel.<div id="exp_DeleteTextChannel">
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

*Source: `ComOff/ChnConvertTextToAssignment.htm`*

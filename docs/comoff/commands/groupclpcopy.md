---
title: "GroupClpCopy"
description: "Copies one or more channel groups from the Data Portal to the clipboard."
---

# GroupClpCopy

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GroupClpCopy

Copies one or more channel groups from the Data Portal to the clipboard.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Avoid using the Windows clipboard in scripts, especially in loops. Timely access to the clipboard is unpredictable and may lead to unexpected behavior. Use the <a href="../groupcopy/">GroupCopy</a> command to copy channel groups and to paste channel groups to a new position in the Data Portal. When you use the <span class="Monospace">GroupClpCopy</span> command to copy channel groups to the clipboard, DIAdem copies only a reference. If you modify channels in the channel group, add new channels, or delete channels, DIAdem uses the <a href="../groupclppaste/">GroupClpPaste</a> command to paste the current status of the Data Portal.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ClpSourceData</td>
<td>Specifies the group name or the group index, or the array with the group names, that DIAdem copies.<div id="exp_ClpSourceData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">[ChnXYRelation]</td>
<td>Specifies that x-channel references are used when copying and moving xy-channels and are preserved during reduced loading of xy-channels.<div id="exp_ChnXYRelation">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean</a></td></tr>
<tr>
<td><br attr="ext"/>Access: Read/Write</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is an <a href="#" data-unresolved="1">Integer variable</a> type. Receives the number of copied groups.</td></tr>
</table>
</div>

---

*Source: `ComOff/GroupClpCopy.htm`*

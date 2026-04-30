---
title: "GroupClpPaste"
description: "Pastes one or more channel groups from the clipboard to the Data Portal."
---

# GroupClpPaste

!!! abstract "Command &middot; `ComOff.chm`"
    Command: GroupClpPaste

Pastes one or more channel groups from the clipboard to the Data Portal.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If a command generates a channel group, specify the value 0 to create a channel group after the last channel group.</td></tr></table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Avoid using the Windows clipboard in scripts, especially in loops. Timely access to the clipboard is unpredictable and may lead to unexpected behavior. Use the <a href="../groupcopy/">GroupCopy</a> command to copy channel groups and to paste channel groups to a new position in the Data Portal. When you use the <span class="Monospace">GroupClpCopy</span> command to copy channel groups to the clipboard, DIAdem copies only a reference. If you modify channels in the channel group, add new channels, or delete channels, DIAdem uses the <a href="./">GroupClpPaste</a> command to paste the current status of the Data Portal.<br attr="ext"/></td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">TargetGroupIndex</td>
<td>Specifies the index of a target channel group in the Data Portal.<div id="exp_TargetGroupIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Integer variable</a></td></tr>
<tr>
<td>0 &lt;= TargetGroupIndex &lt;= <a href="../../../varoff/variables/groupcount/">GroupCount</a></td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If a command generates a channel group, specify the value 0 to create a channel group after the last channel group.</td></tr></table>
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
<td>The return value is a <a href="#" data-unresolved="1">Variant variable</a> type. Receives the field with the names of the new groups. The value is NULL <!-- Translate as NULL not Zero -->if DIAdem has not copied a group.</td></tr>
</table>
</div>

---

*Source: `ComOff/GroupClpPaste.htm`*

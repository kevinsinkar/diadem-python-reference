---
title: "ItemInfoGet"
description: "Provides information about a DIAdem variable or a DIAdem command."
---

# ItemInfoGet

!!! abstract "Command &middot; `ComOff.chm`"
    Command: ItemInfoGet

Provides information about a DIAdem variable or a DIAdem command.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>Refer to the page about <a href="#" data-unresolved="1">Variable Types</a> for a description of the variable types.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ItemName</td>
<td>Specifies the name of a DIAdem variable or of a DIAdem command.<div id="exp_ItemName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>The return value is a <a href="#" data-unresolved="1">Boolean</a> type. The value is <span class="Monospace">TRUE</span> if DIAdem could determine information about the variable or command, otherwise the value is <span class="Monospace">FALSE</span>.</td></tr>
</table>
</div>

---

*Source: `ComOff/ItemInfoGet.htm`*

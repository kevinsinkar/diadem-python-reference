---
title: "DCSDoIPEntityAddress"
description: "Specifies the address of one of the DoIP units in the list."
---

# DCSDoIPEntityAddress

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPEntityAddress

Specifies the address of one of the DoIP units in the list.

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Because only three bytes are reserved for the transmission to the ECU, the storage address must be in the range between <span class="Monospace">0</span> and <span class="Monospace">FFFFFF</span>.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDoIPEntityList</td>
<td>Specifies a list with DoIP units (vehicles) from the local sub-net.<div id="exp_DCSDoIPEntityList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">DCSListIndex</td>
<td>Specifies the index in the list.<div id="exp_DCSListIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the logical address of a DoIP unit or the storage address of the data to be read and written. The return value is a DCSAddress type.<div id="exp_DCSAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Because only three bytes are reserved for the transmission to the ECU, the storage address must be in the range between <span class="Monospace">0</span> and <span class="Monospace">FFFFFF</span>.</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPEntityAddress.htm`*

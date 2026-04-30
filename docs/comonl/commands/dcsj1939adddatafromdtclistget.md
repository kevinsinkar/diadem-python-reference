---
title: "DCSJ1939AddDataFromDTCListGet"
description: "Reads additional data of DTCs from a J1939 Diagnostic Trouble Code (DTCs) list."
---

# DCSJ1939AddDataFromDTCListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSJ1939AddDataFromDTCListGet

Reads additional data of DTCs from a J1939 Diagnostic Trouble Code (DTCs) list.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSWWHDTCJ1939List</td>
<td>Specifies the list of DTCs in the J1939 format.<div id="exp_DCSWWHDTCJ1939List">
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
<td>Receives the additional DTC data. Type DCSWWHAddData return value.<div id="exp_DCSWWHAddData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSJ1939AddDataFromDTCListGet.htm`*

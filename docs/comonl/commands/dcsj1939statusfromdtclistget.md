---
title: "DCSJ1939StatusFromDTCListGet"
description: "Reads the status of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J1939 format."
---

# DCSJ1939StatusFromDTCListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSJ1939StatusFromDTCListGet

Reads the status of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J1939 format.

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
<td>Receives the status of a single DTC. Type DCSWWHStatus return value.<div id="exp_DCSWWHStatus">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSJ1939StatusFromDTCListGet.htm`*

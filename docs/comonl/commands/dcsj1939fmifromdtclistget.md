---
title: "DCSJ1939FMIFromDTCListGet"
description: "Reads the Failure Mode Identifier (FMI) of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J1939 format."
---

# DCSJ1939FMIFromDTCListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSJ1939FMIFromDTCListGet

Reads the Failure Mode Identifier (FMI) of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J1939 format.

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
<td>Receives the Failure Mode Identifier (FMI) for an individual DTC. Type DCSWWHFMI return value.<div id="exp_DCSWWHFMI">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSJ1939FMIFromDTCListGet.htm`*

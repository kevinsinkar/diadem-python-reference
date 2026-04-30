---
title: "DCSJ2012FTBFromDTCListGet"
description: "Reads a Failure Type Byte (FTB) of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J2012 format."
---

# DCSJ2012FTBFromDTCListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSJ2012FTBFromDTCListGet

Reads a Failure Type Byte (FTB) of an individual DTC from a Diagnostic Trouble Code (DTC) list which is in J2012 format.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSWWHDTCJ2012List</td>
<td>Specifies the list of DTCs in the J2012 format.<div id="exp_DCSWWHDTCJ2012List">
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
<td>Receives the failure type byte (FTB) of a single DTC. Type DCSWWHFTB return value.<div id="exp_DCSWWHFTB">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSJ2012FTBFromDTCListGet.htm`*

---
title: "DCSWWHSupportedRIDsRequest"
description: "Executes the WWH-OBD RoutineControl-Service service in order to get a list of the supported RIDs."
---

# DCSWWHSupportedRIDsRequest

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSWWHSupportedRIDsRequest

Executes the WWH-OBD RoutineControl-Service service in order to get a list of the supported RIDs.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDiagRef</td>
<td>Specifies the diagnostic handle in a vehicle.<div id="exp_DCSDiagRef">
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
<td>Receives a list of valid RIDs. Type DCSWWHRIDList return value.<div id="exp_DCSWWHRIDList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSWWHSupportedRIDsRequest.htm`*

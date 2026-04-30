---
title: "DCSWWHSupportedDIDsRequest"
description: "Executes the WWH-OBD ReadDataByIdentifier service in order to get a list of the supported DIDs."
---

# DCSWWHSupportedDIDsRequest

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSWWHSupportedDIDsRequest

Executes the WWH-OBD ReadDataByIdentifier service in order to get a list of the supported DIDs.

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
<tr><td width="150">DCSWWHDID</td>
<td>Specifies the Diagnostic Data Identifier for this service.<div id="exp_DCSWWHDID">
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
<td>Receives a list of valid DIDs. Type DCSWWHDIDList return value.<div id="exp_DCSWWHDIDList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSWWHSupportedDIDsRequest.htm`*

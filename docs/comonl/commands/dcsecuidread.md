---
title: "DCSECUIDRead"
description: "Reads the engine control unit (ECU) ID."
---

# DCSECUIDRead

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSECUIDRead

Reads the engine control unit (ECU) ID.

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
<tr><td width="150">DCSECUIDReadMode</td>
<td>Specifies the ID type to be transferred. The application determines the settings.<div id="exp_DCSECUIDReadMode">
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
<td>Receives the user-defined date for a service. The return value is a DCSData type.<div id="exp_DCSData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSECUIDRead.htm`*

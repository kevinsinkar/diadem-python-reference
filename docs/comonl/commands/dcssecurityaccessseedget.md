---
title: "DCSSecurityAccessSeedGet"
description: "Requests in a security prompt a random number (seed) from the engine control unit (ECU) in order to generate a key code (key)."
---

# DCSSecurityAccessSeedGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSSecurityAccessSeedGet

Requests in a security prompt a random number (seed) from the engine control unit (ECU) in order to generate a key code (key).

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
<tr><td width="150">DCSAccessMode</td>
<td>Specifies which security level to release on the engine control unit (ECU).<div id="exp_DCSAccessMode">
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

*Source: `ComOnl/DCSSecurityAccessSeedGet.htm`*

---
title: "DCSDiagnosticServiceExecute"
description: "Executes a diagnosis service. If a specific service from the KWP2000-, UDS- or OBD-service function are not available, you can use this function to call the res"
---

# DCSDiagnosticServiceExecute

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDiagnosticServiceExecute

Executes a diagnosis service. If a specific service from the KWP2000-, UDS- or OBD-service function are not available, you can use this function to call the respective service.

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
<tr><td width="150">DCSResponseRequired</td>
<td>Specifies whether a service requires a response.<div id="exp_DCSResponseRequired">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean Variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSData</td>
<td>Specifies the user-defined date for a service.<div id="exp_DCSData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the user-defined date for a service. The return value is a DCSData type.<div id="exp_DCSData__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDiagnosticServiceExecute.htm`*

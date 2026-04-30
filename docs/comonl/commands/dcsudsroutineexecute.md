---
title: "DCSUDSRoutineExecute"
description: "Executes a routine on the engine control unit (ECU)."
---

# DCSUDSRoutineExecute

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSRoutineExecute

Executes a routine on the engine control unit (ECU).

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
<tr><td width="150">DCSID</td>
<td>Specifies the routine ID.<div id="exp_DCSID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSUDSExecuteMode</td>
<td>Specifies the execution mode of the service.<div id="exp_DCSUDSExecuteMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless">
<tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">01</td><td>Starts the routine</td></tr>
<tr><td align="center" class="Monospace">02</td><td>Stops the routing</td></tr>
<tr><td align="center" class="Monospace">03</td><td>Requests the routine results</td></tr>
<tr><td align="center" class="Monospace">&gt;3</td><td>Application specific</td></tr>
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

*Source: `ComOnl/DCSUDSRoutineExecute.htm`*

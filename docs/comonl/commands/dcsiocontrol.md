---
title: "DCSIOControl"
description: "Controls the behavior of the I/O port of the engine control unit (ECU)."
---

# DCSIOControl

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSIOControl

Controls the behavior of the I/O port of the engine control unit (ECU).

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
<tr><td width="150">DCSLocalId</td>
<td>Specifies the local ID of the I/O port to be controlled.<div id="exp_DCSLocalId">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSIOControlMode</td>
<td>Specifies the I/O control type. The application determines the settings.<div id="exp_DCSIOControlMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Returns the control to the engine control unit</td></tr>
<tr><td align="center" class="Monospace">1</td><td>Status message</td></tr>
<tr><td align="center" class="Monospace">4</td><td>Sets the default value</td></tr>
<tr><td align="center" class="Monospace">5</td><td>Freezes the current status</td></tr>
<tr><td align="center" class="Monospace">7</td><td>Short-term adjustment</td></tr>
<tr><td align="center" class="Monospace">8</td><td>Long-term adjustment</td></tr>
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

*Source: `ComOnl/DCSIOControl.htm`*

---
title: "DCSOBDOpen"
description: "Starts a diagnosis session over a CAN port for OBD-II (on-board diagnostic)."
---

# DCSOBDOpen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSOBDOpen

Starts a diagnosis session over a CAN port for OBD-II (on-board diagnostic).

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSCANHardware</td>
<td>Specifies the CAN hardware.<div id="exp_DCSCANHardware">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">1</td><td>NI-CAN</td></tr><tr><td align="center" class="Monospace">2</td><td>NI-XNET</td></tr><tr><td align="center" class="Monospace">3</td><td>Vector XL Driver</td></tr><tr><td align="center" class="Monospace">4</td><td>Reserved</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSCANInterface</td>
<td>Specifies the name of the CAN interface.<div id="exp_DCSCANInterface">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSBaudRate</td>
<td>Specifies the baud rate.<div id="exp_DCSBaudRate">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSTransmitID</td>
<td>Specifies the CAN ID of the message sent to the engine control unit (ECU).<div id="exp_DCSTransmitID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSReceiveID</td>
<td>Specifies the CAN ID of the message received by the engine control unit (ECU).<div id="exp_DCSReceiveID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the diagnostic handle in a vehicle. The return value is a DCSDiagRef type.<div id="exp_DCSDiagRef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSOBDOpen.htm`*

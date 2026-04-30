---
title: "DCSDiagosticFrameReceive"
description: "Uses a diagnostics-CAN-ID to receive a CAN frame, in order to check the transport log for errors."
---

# DCSDiagosticFrameReceive

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDiagosticFrameReceive

Uses a diagnostics-CAN-ID to receive a CAN frame, in order to check the transport log for errors.

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
<tr><td width="150">DCSTimeout</td>
<td>Specifies the timeout.<div id="exp_DCSTimeout">
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

*Source: `ComOnl/DCSDiagosticFrameReceive.htm`*

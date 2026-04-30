---
title: "DCSUDSTransmit"
description: "Transfers data to the engine control unit (ECU) in an upload process or receives data from an ECU in a download process."
---

# DCSUDSTransmit

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSTransmit

Transfers data to the engine control unit (ECU) in an upload process or receives data from an ECU in a download process.

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
<tr><td width="150">DCSBlockSequenceCounter</td>
<td>Specifies the number of the data block being transferred.<div id="exp_DCSBlockSequenceCounter">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">After the initialization of the data transfer, the counter starts with the value <span class="Monospace">1</span> and runs to the value <span class="Monospace">255</span>. Then the counter is set to the value <span class="Monospace">0</span>.</p>
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

*Source: `ComOnl/DCSUDSTransmit.htm`*

---
title: "DCSDoIPOpen"
description: "Starts a diagnosis session through the IP address without starting the communication with the engine control unit (ECU)."
---

# DCSDoIPOpen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPOpen

Starts a diagnosis session through the IP address without starting the communication with the engine control unit (ECU).

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDynamicPort</td>
<td>Specifies which UDP port to use for the communication.<div id="exp_DCSDynamicPort">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean Variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">False</td><td>Standard UDP port 13401</td></tr><tr><td align="center" class="Monospace">True</td><td>Dynamically assigned UDP port</td></tr></table>
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

*Source: `ComOnl/DCSDoIPOpen.htm`*

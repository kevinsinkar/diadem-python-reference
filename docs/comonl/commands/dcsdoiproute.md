---
title: "DCSDoIPRoute"
description: "Specifies the source and destination address of a TCP/IP connection with a DoIP unit."
---

# DCSDoIPRoute

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPRoute

Specifies the source and destination address of a TCP/IP connection with a DoIP unit.

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
<tr><td width="150">DCSDoIPActivationType</td>
<td>Specifies the enabling type which requires different types of authentication and/or confirmation.<div id="exp_DCSDoIPActivationType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Standard</td></tr><tr><td align="center" class="Monospace">1</td><td>WWH - OBD (worldwide unified automatic diagnostic)</td></tr><tr><td align="center" class="Monospace">2 - 0xDF</td><td>Reserved</td></tr><tr><td align="center" class="Monospace">0xE0</td><td>OEM specific safety approach</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSSourceAddress</td>
<td>Specifies the DoIP source address of the tester that starts the communication.<div id="exp_DCSSourceAddress">
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
<td>Receives the target address. The return value is a DCSTargetAddress type.<div id="exp_DCSTargetAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPRoute.htm`*

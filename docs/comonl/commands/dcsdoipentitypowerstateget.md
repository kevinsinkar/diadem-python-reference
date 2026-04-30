---
title: "DCSDoIPEntityPowerStateGet"
description: "Specifies the diagnosis status of a DoIP unit."
---

# DCSDoIPEntityPowerStateGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPEntityPowerStateGet

Specifies the diagnosis status of a DoIP unit.

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
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the diagnosis status. The return value is a DCSDoIPPowerState type.<div id="exp_DCSDoIPPowerState">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Not ready</td></tr><tr><td align="center" class="Monospace">1</td><td>Ready</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPEntityPowerStateGet.htm`*

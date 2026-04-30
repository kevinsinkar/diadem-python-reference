---
title: "DCSDoIPEntityStatusNodeType"
description: "Determines the type of a DoIP unit from the DCSDoIPEntityStatus data structure."
---

# DCSDoIPEntityStatusNodeType

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPEntityStatusNodeType

Determines the type of a DoIP unit from the DCSDoIPEntityStatus data structure.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDoIPEntityStatus</td>
<td>Specifies the status of the DoIP unit.<div id="exp_DCSDoIPEntityStatus">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">Use the functions <a href="../dcsdoipentitystatuscurrentsockets/">DCSDoIPEntityStatusCurrentSockets</a>, <a href="../dcsdoipentitystatusmaxsockets/">DCSDoIPEntityStatusMaxSockets</a> and <a href="./">DCSDoIPEntityStatusNodeType</a> to determine the individual status information from this parameter.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Specifies the type of a DoIP unit. The return value is a DCSDoIPEntityNodeType type.<div id="exp_DCSDoIPEntityNodeType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>DoIP gateway</td></tr><tr><td align="center" class="Monospace">1</td><td>DoIP unit</td></tr><tr><td align="center" class="Monospace">&gt;1</td><td>Reserved</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPEntityStatusNodeType.htm`*

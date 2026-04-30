---
title: "DCSDoIPEntityStatusMaxSockets"
description: "Determines the maximum number of TCP/IP sockets of a DoIP unit from the DCSDoIPEntityStatus data structure."
---

# DCSDoIPEntityStatusMaxSockets

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPEntityStatusMaxSockets

Determines the maximum number of TCP/IP sockets of a DoIP unit from the DCSDoIPEntityStatus data structure.

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
<p class="body">Use the functions <a href="../dcsdoipentitystatuscurrentsockets/">DCSDoIPEntityStatusCurrentSockets</a>, <a href="./">DCSDoIPEntityStatusMaxSockets</a> and <a href="../dcsdoipentitystatusnodetype/">DCSDoIPEntityStatusNodeType</a> to determine the individual status information from this parameter.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the maximum number of TCP/IP sockets of the DoIP unit. The return value is a DCSDoIPEntityMaxSockets type.<div id="exp_DCSDoIPEntityMaxSockets">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPEntityStatusMaxSockets.htm`*

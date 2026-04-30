---
title: "DCSDoIPEntityStatusGet"
description: "Specifies the status of a DoIP unit."
---

# DCSDoIPEntityStatusGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPEntityStatusGet

Specifies the status of a DoIP unit.

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
<td>Receives the status of the DoIP unit. The return value is a DCSDoIPEntityStatus type.<div id="exp_DCSDoIPEntityStatus">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">Use the functions <a href="../dcsdoipentitystatuscurrentsockets/">DCSDoIPEntityStatusCurrentSockets</a>, <a href="../dcsdoipentitystatusmaxsockets/">DCSDoIPEntityStatusMaxSockets</a> and <a href="../dcsdoipentitystatusnodetype/">DCSDoIPEntityStatusNodeType</a> to determine the individual status information from this parameter.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPEntityStatusGet.htm`*

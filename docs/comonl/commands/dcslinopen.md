---
title: "DCSLINOpen"
description: "Opens a diagnosis session on an NI-XNET LIN port."
---

# DCSLINOpen

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSLINOpen

Opens a diagnosis session on an NI-XNET LIN port.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSLINInterface</td>
<td>Specifies the NI-XNET LIN interface to be used for communication.<div id="exp_DCSLINInterface">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSLINDBAlias</td>
<td>Specifies the NI-XNET database alias to be used.<div id="exp_DCSLINDBAlias">
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
<tr><td width="150">DCSLINMasterReqFrame</td>
<td>Specifies the request frame of the master device from the LDF or FIBEX database.<div id="exp_DCSLINMasterReqFrame">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSLINSlaveRespFrame</td>
<td>Specifies the answer frame of the slave device from the LDF or FIBEX database.<div id="exp_DCSLINSlaveRespFrame">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSLINNAD</td>
<td>Contains the address of the addressed slave node.<div id="exp_DCSLINNAD">
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
<td>Specifies the diagnostic handle in a vehicle. The return value is a DCSDiagRef type.<div id="exp_DCSDiagRef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSLINOpen.htm`*

---
title: "DCSOBDPowertrainDTCFreezedDataGet"
description: "Executes an OBD request current powertrain freeze frame data service and reads the data that is acquired."
---

# DCSOBDPowertrainDTCFreezedDataGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSOBDPowertrainDTCFreezedDataGet

Executes an OBD request current powertrain freeze frame data service and reads the data that is acquired.

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
<tr><td width="150">DCSParameterID</td>
<td>Specifies the ID of a parameter to be read. The values for this parameter are defined in the SAE J1979 standard.<div id="exp_DCSParameterID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSFrame</td>
<td>Specifies the number of the frame whose data is read.<div id="exp_DCSFrame">
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

*Source: `ComOnl/DCSOBDPowertrainDTCFreezedDataGet.htm`*

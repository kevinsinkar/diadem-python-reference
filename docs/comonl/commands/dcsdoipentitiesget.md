---
title: "DCSDoIPEntitiesGet"
description: "Specifies a table with the DoIP units (vehicles) of the local sub-net which refers to the entity ID (EID) or the vehicle ID number (VIN)."
---

# DCSDoIPEntitiesGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPEntitiesGet

Specifies a table with the DoIP units (vehicles) of the local sub-net which refers to the entity ID (EID) or the vehicle ID number (VIN).

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
<tr><td width="150">DCSDoIPEntityType</td>
<td>Specifies the search mode.<div id="exp_DCSDoIPEntityType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Vehicle ID Number (VIN)</td></tr><tr><td align="center" class="Monospace">1</td><td>Entity ID (EID)</td></tr><tr><td align="center" class="Monospace">2</td><td>All (the <a href="../../../varonl/variables/dcsvehicleidnumberorentityid/">DCSVehicleIDNumberOrEntityID</a> parameter is ignored.)</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSVehicleIDNumberOrEntityID</td>
<td>Specifies the vehicle ID number (VIN) or the entity ID (EID).<div id="exp_DCSVehicleIDNumberOrEntityID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives a list with DoIP units (vehicles) from the local sub-net. The return value is a DCSDoIPEntityList type.<div id="exp_DCSDoIPEntityList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPEntitiesGet.htm`*

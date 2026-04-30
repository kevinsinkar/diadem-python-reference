---
title: "DCSDoIPVehicleIDByEntityIDRequest"
description: "Sends an UDP request with an entity ID (EID) to all DoIP capable devices in a sub-net so that these devices can identify themselves."
---

# DCSDoIPVehicleIDByEntityIDRequest

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPVehicleIDByEntityIDRequest

Sends an UDP request with an entity ID (EID) to all DoIP capable devices in a sub-net so that these devices can identify themselves.

## Signature

```python
dd.DCSDoIPVehicleIDByEntityIDRequest(DCSDiagRef, DCSVehicleIDNumberOrEntityID)
```

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

---

*Source: `ComOnl/DCSDoIPVehicleIDByEntityIDRequest.htm`*

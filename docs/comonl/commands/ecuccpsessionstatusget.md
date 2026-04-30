---
title: "ECUCCPSessionStatusGet"
description: "Retrieves the current status of the calibration session (CCP only)."
---

# ECUCCPSessionStatusGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCCPSessionStatusGet

Retrieves the current status of the calibration session (CCP only).

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUDeviceHandle</td>
<td>Specifies the handle for the ECU.<div id="exp_ECUDeviceHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUDeviceHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Contains the current status of the ECU calibration as a bit mask which contains several session statuses of the ECU. The return value is a ECUSessionStatus type.<div id="exp_ECUSessionStatus">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUSessionStatus &lt;= 255</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCCPSessionStatusGet.htm`*

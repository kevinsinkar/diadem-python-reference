---
title: "ECUXCPStatusGet"
description: "Queries the current session status of an ECU slave device."
---

# ECUXCPStatusGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPStatusGet

Queries the current session status of an ECU slave device.

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
<td>Receives the current status of the ECU calibration as a bit mask which contains several session statuses of the ECU. ECUStatusQualifier and ECUAdditionalStatus contain additional status information. The contents of these values is ECU specific and not defined by CCP. The return value is a ECUSessionStatus type.<div id="exp_ECUSessionStatus">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUSessionStatus &lt;= 255</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPStatusGet.htm`*

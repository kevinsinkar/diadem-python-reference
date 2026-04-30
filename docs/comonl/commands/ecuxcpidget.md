---
title: "ECUXCPIdGet"
description: "Retrieves the session configuration or the slave device identification."
---

# ECUXCPIdGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPIdGet

Retrieves the session configuration or the slave device identification.

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
<tr><td width="150">ECUXCPIdSelector</td>
<td>Specifies the type of requested identification.<div id="exp_ECUXCPIdSelector">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
<td>0 &lt;= ECUXCPIDSelector &lt;= 4</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the requested ID string. The return value is a ECUXCPId type.<div id="exp_ECUXCPId">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPIdGet.htm`*

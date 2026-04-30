---
title: "ECUCCPCalibPageGet"
description: "Determines the address of the active data calibration page."
---

# ECUCCPCalibPageGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCCPCalibPageGet

Determines the address of the active data calibration page.

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
<td>Contains the address part of the data calibration page. The return value is a ECUSourceAddress type.<div id="exp_ECUSourceAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUSourceAddress &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCCPCalibPageGet.htm`*

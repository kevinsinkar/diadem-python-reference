---
title: "ECUXCPCalibPageGet"
description: "Retrieves a setting of the calibration page."
---

# ECUXCPCalibPageGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPCalibPageGet

Retrieves a setting of the calibration page.

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
<tr><td width="150">ECUMode</td>
<td>Specifies a bit mask which describes the mode.<div id="exp_ECUMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUSegment</td>
<td>Specifies the logical number of the data segment.<div id="exp_ECUSegment">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Returns the logical page number. The return value is a ECUPage type.<div id="exp_ECUPage">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPCalibPageGet.htm`*

---
title: "ECUCharacteristicSingleValueGet"
description: "Reads a single value from a specific Characteristic on the ECU which is identified by the ECU reference handle."
---

# ECUCharacteristicSingleValueGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCharacteristicSingleValueGet

Reads a single value from a specific Characteristic on the ECU which is identified by the ECU reference handle.

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
<tr><td width="150">ECUName</td>
<td>Specifies the name for accessing an element in an A2L database file. This name is, for example, the name of an ECU, a Characteristic, or a Measurement.<div id="exp_ECUName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUColIndex</td>
<td>Specifies the horizontal index when the characteristic is one dimensional or two dimensional.<div id="exp_ECUColIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUColIndex &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECURowIndex</td>
<td>Specifies the vertical index when the characteristic is two dimensional.<div id="exp_ECURowIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECURowIndex &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Contains a single value. The return value is a ECUValue type.<div id="exp_ECUValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCharacteristicSingleValueGet.htm`*

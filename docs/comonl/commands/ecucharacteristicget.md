---
title: "ECUCharacteristicGet"
description: "Reads all data from a specific characteristic on the ECU which is identified by the ECU Reference handle."
---

# ECUCharacteristicGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCharacteristicGet

Reads all data from a specific characteristic on the ECU which is identified by the ECU Reference handle.

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
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Contains a single value or a one or two dimensional array of values for the selected characteristic. The return value is a ECUCharacteristicData type.<div id="exp_ECUCharacteristicData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCharacteristicGet.htm`*

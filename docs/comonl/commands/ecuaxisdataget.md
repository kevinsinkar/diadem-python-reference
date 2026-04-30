---
title: "ECUAxisDataGet"
description: "Reads the values at the x-axis or y-axis of a characteristic."
---

# ECUAxisDataGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUAxisDataGet

Reads the values at the x-axis or y-axis of a characteristic.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUHandle</td>
<td>Specifies the handle you use to access the ECU.<div id="exp_ECUHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUHandle &lt;= 2147483647</td></tr>
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
<tr><td width="150">ECUAxisSelector</td>
<td>Specifies the axis. The engine control unit (ECU) reads the respective values.<div id="exp_ECUAxisSelector">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUAxisSelector &lt;= 1</td></tr>
</table>The <span class="Monospace">ECUAxisSelector</span> variable can use the following constants:<table class="Borderless">
<tr><td>0</td><td width="150"><span class="Monospace">eECUAxisX</span></td><td>Read out x-axis values.</td></tr>
<tr><td>1</td><td width="150"><span class="Monospace">eECUAxisY</span></td><td>Read out y-axis values.</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Contains a single value or a one dimensional array of values for the selected Characteristic. The return value is a ECUCharacteristicData type.<div id="exp_ECUCharacteristicData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eECUAxisX` | 0 | Read out x-axis values. |
| `eECUAxisY` | 1 | Read out y-axis values. |

---

*Source: `ComOnl/ECUAxisDataGet.htm`*

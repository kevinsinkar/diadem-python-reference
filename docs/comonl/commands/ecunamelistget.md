---
title: "ECUNameListGet"
description: "Calls a list with the names of all ECUs, Measurements, Characteristics, Events, Characteristic pages, or Groups from a specified A2L database."
---

# ECUNameListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUNameListGet

Calls a list with the names of all ECUs, Measurements, Characteristics, Events, Characteristic pages, or Groups from a specified A2L database.

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
<tr><td width="150">ECUNameSelector</td>
<td>Specifies the type to be returned.<div id="exp_ECUNameSelector">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUNameSelector &lt;= 20</td></tr>
</table>
<p class="body">The variable can accept the following values:</p>
<table class="Borderless">
<tr><td>0</td><td width="150"><span class="Monospace">eECUNamesECUs</span></td><td>All ECUs defined in the A2L file</td></tr>
<tr><td>1</td><td width="150"><span class="Monospace">eECUNamesMeasurements</span></td><td>All measurements defined in the A2L file</td></tr>
<tr><td>2</td><td width="150"><span class="Monospace">eECUNamesCharacteristics</span></td><td>All characteristics defined in the A2L file</td></tr>
<tr><td>3</td><td width="150"><span class="Monospace">eECUNamesEventChannels</span></td><td>All event channels defined in the A2L file</td></tr>
<tr><td>4</td><td width="150"><span class="Monospace">eECUNamesDefinedPages</span></td><td>All memory pages defined in the A2L file</td></tr>
<tr><td>5</td><td width="150"><span class="Monospace">eECUNamesGroups</span></td><td>All groups defined in the A2L file</td></tr>
<tr><td>6</td><td width="150"><span class="Monospace">eECUNamesSubGroups</span></td><td>All subgroups defined in the <span class="Monospace">ECUName</span> group</td></tr>
<tr><td>7</td><td width="150"><span class="Monospace">eECUNamesGroupMeasurements</span></td><td>All measurements defined in the <span class="Monospace">ECUName</span> group</td></tr>
<tr><td>8</td><td width="150"><span class="Monospace">eECUNamesGroupCharacteristics</span></td><td>All characteristics defined in the <span class="Monospace">ECUName</span> group</td></tr></table>
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
<td>Contains a list of names separated by commas from the specified type. The return value is a ECUNameList type.<div id="exp_ECUNameList">
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
| `eECUNamesECUs` | 0 | All ECUs defined in the A2L file |
| `eECUNamesMeasurements` | 1 | All measurements defined in the A2L file |
| `eECUNamesCharacteristics` | 2 | All characteristics defined in the A2L file |
| `eECUNamesEventChannels` | 3 | All event channels defined in the A2L file |
| `eECUNamesDefinedPages` | 4 | All memory pages defined in the A2L file |
| `eECUNamesGroups` | 5 | All groups defined in the A2L file |
| `eECUNamesSubGroups` | 6 | All subgroups defined in the ECUName group |
| `eECUNamesGroupMeasurements` | 7 | All measurements defined in the ECUName group |
| `eECUNamesGroupCharacteristics` | 8 | All characteristics defined in the ECUName group |

---

*Source: `ComOnl/ECUNameListGet.htm`*

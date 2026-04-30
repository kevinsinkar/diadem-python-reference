---
title: "ECUCharacteristicSingleValueSet"
description: "Transfers a single value of a Characteristic to a selected ECU."
---

# ECUCharacteristicSingleValueSet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCharacteristicSingleValueSet

Transfers a single value of a Characteristic to a selected ECU.

## Signature

```python
dd.ECUCharacteristicSingleValueSet(ECUDeviceHandle, ECUName, ECUColIndex, ECURowIndex, ECUValue)
```

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
<tr><td width="150">ECUValue</td>
<td>Specifies a value<div id="exp_ECUValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCharacteristicSingleValueSet.htm`*

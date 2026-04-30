---
title: "ECUConnect"
description: "Establishes communication to the selected ECU through CCP or XCP. After a successful ECU connect you can create a measurement task or read/write a characteristi"
---

# ECUConnect

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUConnect

Establishes communication to the selected ECU through CCP or XCP. After a successful ECU connect you can create a measurement task or read/write a characteristic.

## Signature

```python
dd.ECUConnect(ECUDeviceHandle)
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
</table>
</div>

---

*Source: `ComOnl/ECUConnect.htm`*

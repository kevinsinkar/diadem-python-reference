---
title: "ECUProgram"
description: "Programs a memory block on the ECU."
---

# ECUProgram

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUProgram

Programs a memory block on the ECU.

## Signature

```python
dd.ECUProgram(ECUDeviceHandle, ECUTargetAddress, ECUTargetExtension, ECUData)
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
<tr><td width="150">ECUTargetAddress</td>
<td>Specifies the address part of the destination address.<div id="exp_ECUTargetAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUTargetAddress &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUTargetExtension</td>
<td>Contains the extension part of the destination address.<div id="exp_ECUTargetExtension">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUData</td>
<td>Contains the data which the ECU read or received.<div id="exp_ECUData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUProgram.htm`*

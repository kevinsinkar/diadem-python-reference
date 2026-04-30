---
title: "ECUXCPProgramPrepare"
description: "Prepares the programming of non-volatile memory."
---

# ECUXCPProgramPrepare

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPProgramPrepare

Prepares the programming of non-volatile memory.

## Signature

```python
dd.ECUXCPProgramPrepare(ECUDeviceHandle, ECUTargetAddress, ECUTargetExtension, ECUCodeSize)
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
<tr><td width="150">ECUCodeSize</td>
<td>Specifies the size of the data to be downloaded.<div id="exp_ECUCodeSize">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUCodeSize &lt;= 65535</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPProgramPrepare.htm`*

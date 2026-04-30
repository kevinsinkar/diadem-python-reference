---
title: "ECUCCPMemoryMove"
description: "Moves a memory block on the ECU (CCP only)."
---

# ECUCCPMemoryMove

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCCPMemoryMove

Moves a memory block on the ECU (CCP only).

## Signature

```python
dd.ECUCCPMemoryMove(ECUDeviceHandle, ECUSourceAddress, ECUSourceExtension, ECUTargetAddress, ECUTargetExtension, ECUBlockSize)
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
<tr><td width="150">ECUSourceAddress</td>
<td>Specifies the address part of the source address.<div id="exp_ECUSourceAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUSourceAddress &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUSourceExtension</td>
<td>Specifies the extension part of the source address.<div id="exp_ECUSourceExtension">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
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
<tr><td width="150">ECUBlockSize</td>
<td>Specifies the block size in bytes.<div id="exp_ECUBlockSize">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUBlockSize &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCCPMemoryMove.htm`*

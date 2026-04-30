---
title: "ECUXCPProgramVerify"
description: "Performs a non-volatile memory certification task on the ECU."
---

# ECUXCPProgramVerify

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUXCPProgramVerify

Performs a non-volatile memory certification task on the ECU.

## Signature

```python
dd.ECUXCPProgramVerify(ECUDeviceHandle, ECUMode, ECUVerificationType, ECUVerificationValue)
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
<tr><td width="150">ECUMode</td>
<td>Specifies a bit mask which describes the mode.<div id="exp_ECUMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUVerificationType</td>
<td>Specifies the type of the requested program verification as a bit mask.<div id="exp_ECUVerificationType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUVerificationType &lt;= 65535</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUVerificationValue</td>
<td>Specifies the verification value if the value of the ECU mode is 1<div id="exp_ECUVerificationValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUVerificationValue &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUXCPProgramVerify.htm`*

---
title: "DCSSecurityAccessKeySend"
description: "Sends a security check of a key code to the engine control unit (ECU)."
---

# DCSSecurityAccessKeySend

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSSecurityAccessKeySend

Sends a security check of a key code to the engine control unit (ECU).

## Signature

```python
dd.DCSSecurityAccessKeySend(DCSDiagRef, DCSAccessMode, DCSData)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDiagRef</td>
<td>Specifies the diagnostic handle in a vehicle.<div id="exp_DCSDiagRef">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSAccessMode</td>
<td>Specifies which security level to release on the engine control unit (ECU).<div id="exp_DCSAccessMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSData</td>
<td>Specifies the user-defined date for a service.<div id="exp_DCSData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSSecurityAccessKeySend.htm`*

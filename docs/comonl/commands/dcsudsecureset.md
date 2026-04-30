---
title: "DCSUDSECUReset"
description: "Resets the engine control unit (ECU)."
---

# DCSUDSECUReset

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSECUReset

Resets the engine control unit (ECU).

## Signature

```python
dd.DCSUDSECUReset(DCSDiagRef, DCSUDSECUResetMode)
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
<tr><td width="150">DCSUDSECUResetMode</td>
<td>Specifies the reset mode of the engine control unit (ECU).<div id="exp_DCSUDSECUResetMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless">
<tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">01</td><td>Cold start</td></tr>
<tr><td align="center" class="Monospace">02</td><td>Key off/on reset. This setting simulates the switching on and off of the ignition with the car key.</td></tr>
<tr><td align="center" class="Monospace">03</td><td>Warm start</td></tr>
<tr><td align="center" class="Monospace">04</td><td>Enables the quick stop</td></tr>
<tr><td align="center" class="Monospace">05</td><td>Disables the quick stop</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSUDSECUReset.htm`*

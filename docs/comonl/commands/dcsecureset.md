---
title: "DCSECUReset"
description: "Restarts the engine control unit (ECU)."
---

# DCSECUReset

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSECUReset

Restarts the engine control unit (ECU).

## Signature

```python
dd.DCSECUReset(DCSDiagRef, DCSECUResetMode)
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
<tr><td width="150">DCSECUResetMode</td>
<td>Specifies the reset mode.<div id="exp_DCSECUResetMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless">
<tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0x01</td><td>Power On</td></tr>
<tr><td align="center" class="Monospace">0x02</td><td>Power On while maintaining the communication</td></tr>
<tr><td align="center" class="Monospace">0x03-0x07F</td><td>Reserved</td></tr>
<tr><td align="center" class="Monospace">0x08-0xFF</td><td>Manufacturer-specific</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSECUReset.htm`*

---
title: "DCSUDSDataWrite"
description: "Uses a local identifier to write data onto the engine control unit (ECU)."
---

# DCSUDSDataWrite

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSDataWrite

Uses a local identifier to write data onto the engine control unit (ECU).

## Signature

```python
dd.DCSUDSDataWrite(DCSDiagRef, DCSID, DCSData)
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
<tr><td width="150">DCSID</td>
<td>Specifies the routine ID.<div id="exp_DCSID">
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

*Source: `ComOnl/DCSUDSDataWrite.htm`*

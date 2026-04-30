---
title: "DCSUDSMemoryWrite"
description: "Writes data into the ECU memory."
---

# DCSUDSMemoryWrite

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSMemoryWrite

Writes data into the ECU memory.

## Signature

```python
dd.DCSUDSMemoryWrite(DCSDiagRef, DCSMemoryAddress, DCSData)
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
<tr><td width="150">DCSMemoryAddress</td>
<td>Specifies the memory address of the data.<div id="exp_DCSMemoryAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
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

*Source: `ComOnl/DCSUDSMemoryWrite.htm`*

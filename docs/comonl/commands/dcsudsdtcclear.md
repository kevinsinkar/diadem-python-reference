---
title: "DCSUDSDTCClear"
description: "Deletes the selected diagnostic trouble codes (DTC)."
---

# DCSUDSDTCClear

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSDTCClear

Deletes the selected diagnostic trouble codes (DTC).

## Signature

```python
dd.DCSUDSDTCClear(DCSDiagRef, DCSGroupOfDTC, DCSDTCDescriptor)
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
<tr><td width="150">DCSGroupOfDTC</td>
<td>Specifies the group of the diagnostic trouble codes.<div id="exp_DCSGroupOfDTC">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0x0000</td><td>All DTCs referring to the power transmission</td></tr>
<tr><td align="center" class="Monospace">0x4000</td><td>All DTCs referring to vehicles</td></tr>
<tr><td align="center" class="Monospace">0x8000</td><td>All DTCs referring to the chassis</td></tr><tr><td align="center" class="Monospace">0xC000</td><td>All DTCs referring to the network</td></tr><tr><td align="center" class="Monospace">0xFF00</td><td>All DTCs</td></tr><tr><td align="center" class="Monospace">0xFFFF</td><td>All DTCs for <a href="./">DCSUDSDTCClear</a></td></tr></table>
<p class="body">All other values are determined by the application.</p>
</div></td></tr>
<tr><td width="150">DCSDTCDescriptor</td>
<td>Specifies the structure of a diagnostic trouble code.<div id="exp_DCSDTCDescriptor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">Use the <a href="../dcsdtcdescriptorinit/">DCSDTCDescriptorInit</a> command to initialize the data structure.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSUDSDTCClear.htm`*

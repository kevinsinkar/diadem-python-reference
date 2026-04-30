---
title: "DCSMemoryWrite"
description: "Writes data into the ECU memory."
---

# DCSMemoryWrite

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSMemoryWrite

Writes data into the ECU memory.

## Signature

```python
dd.DCSMemoryWrite(DCSDiagRef, DCSAddress, DCSData)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Because only three bytes are reserved for the transmission to the ECU, the storage address must be in the range between <span class="Monospace">0</span> and <span class="Monospace">FFFFFF</span>.</td></tr></table>
</div>

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
<tr><td width="150">DCSAddress</td>
<td>Specifies the logical address of a DoIP unit or the storage address of the data to be read and written.<div id="exp_DCSAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<table class="Borderless"><tr><td class="Icon"><img src="image/note.gif"/></td><td><strong>Note  </strong>Because only three bytes are reserved for the transmission to the ECU, the storage address must be in the range between <span class="Monospace">0</span> and <span class="Monospace">FFFFFF</span>.</td></tr></table>
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

*Source: `ComOnl/DCSMemoryWrite.htm`*

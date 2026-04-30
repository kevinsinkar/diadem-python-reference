---
title: "DCSNormalMessageTransmissionStart"
description: "Starts the standard transmission service. The EDU usually transmits CAN messages."
---

# DCSNormalMessageTransmissionStart

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSNormalMessageTransmissionStart

Starts the standard transmission service. The EDU usually transmits CAN messages.

## Signature

```python
dd.DCSNormalMessageTransmissionStart(DCSDiagRef, DCSResponseRequired)
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
<tr><td width="150">DCSResponseRequired</td>
<td>Specifies whether a service requires a response.<div id="exp_DCSResponseRequired">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean Variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSNormalMessageTransmissionStart.htm`*

---
title: "DCSUDSCommunicationModeSet"
description: "Switches the transmission and the reception of normal messages (mostly CAN messages) on or off."
---

# DCSUDSCommunicationModeSet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSCommunicationModeSet

Switches the transmission and the reception of normal messages (mostly CAN messages) on or off.

## Signature

```python
dd.DCSUDSCommunicationModeSet(DCSDiagRef, DCSCommunicationMask, DCSCommunicationType)
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
<tr><td width="150">DCSCommunicationMask</td>
<td>Specifies the data to be transferred.<div id="exp_DCSCommunicationMask">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless">
<tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">00</td><td>Rx on, Tx on</td></tr>
<tr><td align="center" class="Monospace">01</td><td>Rx on, Tx off</td></tr>
<tr><td align="center" class="Monospace">02</td><td>Rx off, Tx on</td></tr>
<tr><td align="center" class="Monospace">03</td><td>Rx off, Tx off</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSCommunicationType</td>
<td>Specifies the application level to be changed.<div id="exp_DCSCommunicationType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">01</td><td>Application</td></tr><tr><td align="center" class="Monospace">02</td><td>Network management</td></tr></table>
<p class="body">You can change several levels at the same time.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSUDSCommunicationModeSet.htm`*

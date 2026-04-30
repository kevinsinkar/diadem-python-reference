---
title: "DCSVWTPConnect"
description: "Creates a connection to the engine control unit (ECU) over the VW TP 2.0 transmission protocol."
---

# DCSVWTPConnect

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSVWTPConnect

Creates a connection to the engine control unit (ECU) over the VW TP 2.0 transmission protocol.

## Signature

```python
dd.DCSVWTPConnect(DCSDiagRef, DCSVWTPChannelID, DCSVWTPApplicationType)
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
<tr><td width="150">DCSVWTPChannelID</td>
<td>Specifies to which CAN message identifier the engine control unit (ECU) answers.<div id="exp_DCSVWTPChannelID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSVWTPApplicationType</td>
<td>Specifies which communication type to use.<div id="exp_DCSVWTPApplicationType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">1</td><td>Diagnosis applications (KWP2000)</td></tr><tr><td align="center" class="Monospace">&lt;&gt;1</td><td>Manufacturer-specific</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSVWTPConnect.htm`*

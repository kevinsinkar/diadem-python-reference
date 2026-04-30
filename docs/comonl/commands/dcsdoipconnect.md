---
title: "DCSDoIPConnect"
description: "Generates a TCP/IP connection to a DoIP unit through the IP address."
---

# DCSDoIPConnect

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDoIPConnect

Generates a TCP/IP connection to a DoIP unit through the IP address.

## Signature

```python
dd.DCSDoIPConnect(DCSDiagRef, DCSIPAddress, DCSSourceAddress, DCSTargetAddress)
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
<tr><td width="150">DCSIPAddress</td>
<td>Specifies the IP address of the engine control unit.<div id="exp_DCSIPAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">DCSSourceAddress</td>
<td>Specifies the DoIP source address of the tester that starts the communication.<div id="exp_DCSSourceAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSTargetAddress</td>
<td>Specifies the destination address.<div id="exp_DCSTargetAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDoIPConnect.htm`*

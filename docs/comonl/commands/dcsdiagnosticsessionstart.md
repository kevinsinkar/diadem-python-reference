---
title: "DCSDiagnosticSessionStart"
description: "Starts a diagnosis and sets the engine control unit (ECU) into diagnostic mode."
---

# DCSDiagnosticSessionStart

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDiagnosticSessionStart

Starts a diagnosis and sets the engine control unit (ECU) into diagnostic mode.

## Signature

```python
dd.DCSDiagnosticSessionStart(DCSDiagRef, DCSSessionStartMode)
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
<tr><td width="150">DCSSessionStartMode</td>
<td>Specifies which diagnosis mode the Engine Control Unit (ECU) is set to. The application determines the settings.<div id="exp_DCSSessionStartMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDiagnosticSessionStart.htm`*

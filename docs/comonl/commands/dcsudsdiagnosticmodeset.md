---
title: "DCSUDSDiagnosticModeSet"
description: "Sets the engine control unit (ECU) into a special diagnosis mode."
---

# DCSUDSDiagnosticModeSet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSDiagnosticModeSet

Sets the engine control unit (ECU) into a special diagnosis mode.

## Signature

```python
dd.DCSUDSDiagnosticModeSet(DCSDiagRef, DCSUDSDiagnosticMode)
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
<tr><td width="150">DCSUDSDiagnosticMode</td>
<td>Specifies which diagnosis mode the Engine Control Unit (ECU) is set to.<div id="exp_DCSUDSDiagnosticMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless">
<tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">01</td><td>Standard session</td></tr>
<tr><td align="center" class="Monospace">02</td><td>ECU programming session</td></tr>
<tr><td align="center" class="Monospace">03</td><td>Extended ECU diagnosis session</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSUDSDiagnosticModeSet.htm`*

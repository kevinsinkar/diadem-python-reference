---
title: "DCSUDSDTCModeSet"
description: "Switches the generation of diagnostic trouble codes (DTC) on or off."
---

# DCSUDSDTCModeSet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSDTCModeSet

Switches the generation of diagnostic trouble codes (DTC) on or off.

## Signature

```python
dd.DCSUDSDTCModeSet(DCSDiagRef, DCSDTCType, DCSData)
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
<tr><td width="150">DCSDTCType</td>
<td>Specifies whether the generation of the Diagnostic Trouble Code (DTC) is active.<div id="exp_DCSDTCType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless">
<tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">1</td><td>Active</td></tr>
<tr><td align="center" class="Monospace">2</td><td>Inactive</td></tr>
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

*Source: `ComOnl/DCSUDSDTCModeSet.htm`*

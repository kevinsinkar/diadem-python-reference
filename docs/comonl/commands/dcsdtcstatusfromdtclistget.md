---
title: "DCSDTCStatusFromDTCListGet"
description: "Determines the DTC status of an element from the list."
---

# DCSDTCStatusFromDTCListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDTCStatusFromDTCListGet

Determines the DTC status of an element from the list.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDTCList</td>
<td>Specifies the list with the diagnostic trouble codes.<div id="exp_DCSDTCList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">DCSListIndex</td>
<td>Specifies the index in the list.<div id="exp_DCSListIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the status of the diagnostic trouble codes. The return value is type <a href="../../../varonl/variables/dcsdtcstatus/">DCSDTCStatus.htm</a>.<div id="exp_DCSDTCStatus">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Test failed</td></tr><tr><td align="center" class="Monospace">1</td><td>Test failed in monitor cycle.</td></tr><tr><td align="center" class="Monospace">2</td><td>Pending DTC</td></tr><tr><td align="center" class="Monospace">3</td><td>Confirmed DTC</td></tr><tr><td align="center" class="Monospace">4</td><td>Test not completed after last deletion</td></tr><tr><td align="center" class="Monospace">5</td><td>Test failed after last deletion</td></tr><tr><td align="center" class="Monospace">6</td><td>Test not complete in monitor cycle.</td></tr><tr><td align="center" class="Monospace">7</td><td>Warning</td></tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDTCStatusFromDTCListGet.htm`*

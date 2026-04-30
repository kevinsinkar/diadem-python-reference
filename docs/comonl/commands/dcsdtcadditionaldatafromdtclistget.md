---
title: "DCSDTCAdditionalDataFromDTCListGet"
description: "Determines the optional additional information on a diagnostic trouble code from a list of DTCs."
---

# DCSDTCAdditionalDataFromDTCListGet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDTCAdditionalDataFromDTCListGet

Determines the optional additional information on a diagnostic trouble code from a list of DTCs.

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
<td>Receives the optional additional information on a diagnostic trouble code (DTC). The return value is a DCSDTCAdditionalData type.<div id="exp_DCSDTCAdditionalData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDTCAdditionalDataFromDTCListGet.htm`*

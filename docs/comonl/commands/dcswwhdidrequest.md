---
title: "DCSWWHDIDRequest"
description: "Reads a data set from the ECU."
---

# DCSWWHDIDRequest

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSWWHDIDRequest

Reads a data set from the ECU.

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
<tr><td width="150">DCSWWHDataIdentifier</td>
<td>Specifies the data identifier of the data to be read. The SAE J1979DA standard determines the values.<div id="exp_DCSWWHDataIdentifier">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSReturnDataAsString</td>
<td>Specifies whether DIAdem returns the result of an ADCS function as a string.<div id="exp_DCSReturnDataAsString">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Boolean variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the user-defined date for a service. The return value is a DCSData type.<div id="exp_DCSData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSWWHDIDRequest.htm`*

---
title: "DCSWWHEmissionDTCsRequest"
description: "Reads the selected diagnostic trouble codes (DTCs)."
---

# DCSWWHEmissionDTCsRequest

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSWWHEmissionDTCsRequest

Reads the selected diagnostic trouble codes (DTCs).

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
<tr><td width="150">DCSSeverityMask</td>
<td>Specifies the information on the severity of diagnostic trouble codes (TDC) to be read.<div id="exp_DCSSeverityMask">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSStatusMask</td>
<td>Specifies the status of the diagnostic trouble codes (TDC) to be read.<div id="exp_DCSStatusMask">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSDTCDescriptor</td>
<td>Specifies the structure of a diagnostic trouble code.<div id="exp_DCSDTCDescriptor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">Use the <a href="../dcsdtcdescriptorinit/">DCSDTCDescriptorInit</a> command to initialize the data structure.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the list with the diagnostic trouble codes. The return value is a DCSDTCList type.<div id="exp_DCSDTCList">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSWWHEmissionDTCsRequest.htm`*

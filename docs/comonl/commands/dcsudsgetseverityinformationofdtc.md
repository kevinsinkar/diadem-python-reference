---
title: "DCSUDSGetSeverityInformationOfDTC"
description: "Executes a weighted status request in order to read selected diagnostic trouble codes (DTC)."
---

# DCSUDSGetSeverityInformationOfDTC

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSGetSeverityInformationOfDTC

Executes a weighted status request in order to read selected diagnostic trouble codes (DTC).

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
<tr><td width="150">DCSDTCMaskRecord</td>
<td>Specifies the status of the diagnostic trouble codes to be read. The values are user-defined.<div id="exp_DCSDTCMaskRecord">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
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

*Source: `ComOnl/DCSUDSGetSeverityInformationOfDTC.htm`*

---
title: "ECUCCPDiagnosticService"
description: "Calls an implementation-specific diagnostic service on the ECU (CCP only)."
---

# ECUCCPDiagnosticService

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUCCPDiagnosticService

Calls an implementation-specific diagnostic service on the ECU (CCP only).

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">ECUDeviceHandle</td>
<td>Specifies the handle for the ECU.<div id="exp_ECUDeviceHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>-21474836487 &lt;= ECUDeviceHandle &lt;= 2147483647</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUServiceNo</td>
<td>Specifies the diagnostic service executed in the ECU.<div id="exp_ECUServiceNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= ECUServiceNo &lt;= 65535</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUServiceParams</td>
<td>Specifies a byte field which you need to execute the diagnosis service by the ECU. The respective ECU implementation determines the parameter definition.<div id="exp_ECUServiceParams">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Contains the result of the service as a byte field. The return value is a ECUServiceResult type.<div id="exp_ECUServiceResult">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUCCPDiagnosticService.htm`*

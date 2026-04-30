---
title: "ECUChecksumCreate"
description: "Calculates the checksum of a data block in the memory."
---

# ECUChecksumCreate

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUChecksumCreate

Calculates the checksum of a data block in the memory.

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
<tr><td width="150">ECUData</td>
<td>Contains the data which the ECU read or received.<div id="exp_ECUData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUChecksumType</td>
<td>Receives the type of the calculated checksum.<div id="exp_ECUChecksumType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the calculated checksum. The return value is a ECUChecksum type.<div id="exp_ECUChecksum">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUChecksum &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUChecksumCreate.htm`*

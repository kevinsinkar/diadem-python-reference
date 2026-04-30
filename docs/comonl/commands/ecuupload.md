---
title: "ECUUpload"
description: "Uploads data from an ECU."
---

# ECUUpload

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: ECUUpload

Uploads data from an ECU.

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
<tr><td width="150">ECUSourceAddress</td>
<td>Specifies the address part of the source address.<div id="exp_ECUSourceAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUSourceAddress &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
<tr><td width="150">ECUSourceExtension</td>
<td>Specifies the extension part of the source address.<div id="exp_ECUSourceExtension">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Byte variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">ECUBlockSize</td>
<td>Specifies the block size in bytes.<div id="exp_ECUBlockSize">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= ECUBlockSize &lt;= 4294967295</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Contains the data from the ECU. The return value is a ECUData type.<div id="exp_ECUData">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/ECUUpload.htm`*

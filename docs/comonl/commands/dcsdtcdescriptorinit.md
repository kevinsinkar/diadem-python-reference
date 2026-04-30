---
title: "DCSDTCDescriptorInit"
description: "Specifies the start of a diagnostic trouble code (DTC)."
---

# DCSDTCDescriptorInit

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSDTCDescriptorInit

Specifies the start of a diagnostic trouble code (DTC).

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDTCCodeLength</td>
<td>Specifies the length of the diagnostic trouble code in bytes.<div id="exp_DCSDTCCodeLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSDTCStatusLength</td>
<td>Specifies the array length of the DTC status and receives the number of array elements.<div id="exp_DCSDTCStatusLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSDTCAdditonalDataLength</td>
<td>Specifies the length of the DTC additional information in bytes.<div id="exp_DCSDTCAdditonalDataLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSByteOrder</td>
<td>Specifies the byte order of the data.<div id="exp_DCSByteOrder">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Motorola format: Big Endian sequence where the most significant byte is stored first</td></tr><tr><td align="center" class="Monospace">1</td><td>Intel format: Little Endian sequence where the least significant byte is stored first</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the structure of a diagnostic trouble code. The return value is a DCSDTCDescriptor type.<div id="exp_DCSDTCDescriptor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">Use the <a href="./">DCSDTCDescriptorInit</a> command to initialize the data structure.</p>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSDTCDescriptorInit.htm`*

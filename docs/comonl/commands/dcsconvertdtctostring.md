---
title: "DCSConvertDTCToString"
description: "Converts a 2-byte diagnostic trouble code (DTC) into a string in compliance with SAE J2012."
---

# DCSConvertDTCToString

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSConvertDTCToString

Converts a 2-byte diagnostic trouble code (DTC) into a string in compliance with SAE J2012.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSDTC</td>
<td>Specifies the diagnostic trouble code (DTC).<div id="exp_DCSDTC">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="Body">You can convert a standard 2-byte DTC with DCSConvertDTCToString into a readable format according to SAE J2012.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the string. DCSString type return value<div id="exp_DCSString">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSConvertDTCToString.htm`*

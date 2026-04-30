---
title: "DCSConvertPhysToBin"
description: "Uses a type description to convert a physical value into a binary number."
---

# DCSConvertPhysToBin

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSConvertPhysToBin

Uses a type description to convert a physical value into a binary number.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSTypeDescriptor</td>
<td>Specifies the parameters for the conversion of binary numbers into physical values and vice versa.<div id="exp_DCSTypeDescriptor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
<p class="body">Use the <a href="../dcstypedescriptorinit/">DCSDTCDescriptorInit</a> command to initialize the data structure.</p>
</div></td></tr>
<tr><td width="150">DCSValue</td>
<td>Specifies the physical value.<div id="exp_DCSValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSData</td>
<td>Specifies the user-defined date for a service.<div id="exp_DCSData">
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
<td>Receives the user-defined date for a service. DCSData type return value.<div id="exp_DCSData__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSConvertPhysToBin.htm`*

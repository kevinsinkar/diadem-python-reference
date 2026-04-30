---
title: "DCSTypeDescriptorInit"
description: "Initializes the DCSTypeDescriptor data structure to convert binary data into physical values and vice versa."
---

# DCSTypeDescriptorInit

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSTypeDescriptorInit

Initializes the DCSTypeDescriptor data structure to convert binary data into physical values and vice versa.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSStartByte</td>
<td>Specifies the position of the first byte of binary data in the data flow.<div id="exp_DCSStartByte">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSByteLength</td>
<td>Specifies the length of the binary value in bytes.<div id="exp_DCSByteLength">
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
<tr><td width="150">DCSDataType</td>
<td>Specifies the data type of the binary data.<div id="exp_DCSDataType">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Unsigned and a maximum of 1 - 4 bytes</td></tr><tr><td align="center" class="Monospace">1</td><td>Signed and a maximum of 1 - 4 bytes</td></tr><tr><td align="center" class="Monospace">2</td><td>Float and Double, 4 or 8 bytes.</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSScaleFactor</td>
<td>Specifies the factor for the conversion into physical values.<div id="exp_DCSScaleFactor">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSScaleOffset</td>
<td>Specifies the offset for the conversion into physical values.<div id="exp_DCSScaleOffset">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the parameters for the conversion of binary numbers into physical values and vice versa. The return value is a DCSTypeDescriptor type.<div id="exp_DCSTypeDescriptor">
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

*Source: `ComOnl/DCSTypeDescriptorInit.htm`*

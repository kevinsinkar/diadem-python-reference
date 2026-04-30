---
title: "DCSUDSDownloadInit"
description: "Initializes the download of data from the engine control unit (ECU)."
---

# DCSUDSDownloadInit

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSUDSDownloadInit

Initializes the download of data from the engine control unit (ECU).

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
<tr><td width="150">DCSMemoryAddress</td>
<td>Specifies the memory address of the data.<div id="exp_DCSMemoryAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSMemorySize</td>
<td>Specifies the memory size of the data block.<div id="exp_DCSMemorySize">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSMemoryAddressLength</td>
<td>Specifies the length of the memory address in bytes.<div id="exp_DCSMemoryAddressLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSMemorySizeLength</td>
<td>Specifies the length of the memory size in bytes.<div id="exp_DCSMemorySizeLength">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSDataFormatIdentifier</td>
<td>Specifies the compression and encoding mode for data transfer.<div id="exp_DCSDataFormatIdentifier">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>No compression and encoding</td></tr><tr><td align="center" class="Monospace">&gt;0</td><td>All other values are not standardized but implementation specific.</td></tr></table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the size of the storage block to be transmitted. The return value is a DCSBlockSize type.<div id="exp_DCSBlockSize">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSUDSDownloadInit.htm`*

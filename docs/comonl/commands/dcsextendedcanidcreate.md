---
title: "DCSExtendedCANIDCreate"
description: "Generates diagnosis-CAN-IDs according to ISO 15765-2."
---

# DCSExtendedCANIDCreate

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSExtendedCANIDCreate

Generates diagnosis-CAN-IDs according to ISO 15765-2.

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSAddressingMode</td>
<td>Specifies the addressing mode.<div id="exp_DCSAddressingMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Physical address</td></tr><tr><td align="center" class="Monospace">1</td><td>Functional addressing</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSTransportProtocol</td>
<td>Specifies the transmission protocol for the transmission of service messages.<div id="exp_DCSTransportProtocol">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>ISO TP Normal mode uses all 8 data bytes</td></tr><tr><td align="center" class="Monospace">1</td><td>ISO TP mixed mode uses the first byte for address extensions</td></tr><tr><td align="center" class="Monospace">2</td><td>VW TP 2.0</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSSourceAddress</td>
<td>Specifies the DoIP source address of the tester that starts the communication.<div id="exp_DCSSourceAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
<tr><td width="150">DCSTargetAddress</td>
<td>Specifies the destination address.<div id="exp_DCSTargetAddress">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150"><em>ReturnValue</em></td>
<td>Receives the CAN-IDs to ISO 15765-2. The return value is a  DCSCANIDs type.<div id="exp_DCSCANIDs">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Variant variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSExtendedCANIDCreate.htm`*

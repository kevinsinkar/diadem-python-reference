---
title: "DCSPropertySet"
description: "Sets a global internal diagnosis property."
---

# DCSPropertySet

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: DCSPropertySet

Sets a global internal diagnosis property.

## Signature

```python
dd.DCSPropertySet(DCSPropertyID, DCSPropertyValue)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">DCSPropertyID</td>
<td>Uses the ID to specify the global internal diagnosis property.<div id="exp_DCSPropertyID">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
<p class="body">The variable can have the following values:</p>
<table class="borderless"><tr><th>Value</th><th>Meaning</th></tr>
<tr><td align="center" class="Monospace">0</td><td>Timeout for diagnosis command in milliseconds (Default: 1000 ms)</td></tr><tr><td align="center" class="Monospace">1</td><td>Timeout for flow control frames in milliseconds (Default: 250 ms)</td></tr><tr><td align="center" class="Monospace">2</td><td>Timeout for consecutive frames in milliseconds (Default: 250 ms)</td></tr><tr><td align="center" class="Monospace">3</td><td>Number of consecutive frames in a block (Default: 0 - all)</td></tr><tr><td align="center" class="Monospace">4</td><td>Minimum time interval between two consecutive frames in milliseconds (Default: 5 ms)</td></tr><tr><td align="center" class="Monospace">5</td><td>Number of wait frames after which the connection is interrupted (Default: 10)</td></tr><tr><td align="center" class="Monospace">6</td><td>Number of transmitted wait frames before each transmitted consecutive frame (Default: 0)</td></tr><tr><td align="center" class="Monospace">7</td><td>Time interval between two wait frames in milliseconds (Default: 25)</td></tr><tr><td align="center" class="Monospace">8</td><td>Filling of the CAN frames: 0 - less than 8 bytes, 1 - always 8 bytes (Default: 1)</td></tr><tr><td align="center" class="Monospace">9</td><td>Padding bytes for the 8-byte frames (Default: 255)</td></tr><tr><td align="center" class="Monospace">10</td><td>Erroneous ECU reply: 0 - False success (Default), 1 - Error</td></tr><tr><td align="center" class="Monospace">11</td><td>Number of pending replies until cancellation (Default: 5)</td></tr><tr><td align="center" class="Monospace">12</td><td>VWTP command timeout in milliseconds (Default: 50 ms)</td></tr></table>
</div></td></tr>
<tr><td width="150">DCSPropertyValue</td>
<td>Specifies the value of the global internal diagnosis property.<div id="exp_DCSPropertyValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>Access: Read only</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/DCSPropertySet.htm`*

---
title: "OPCSetErrAction"
description: "Specifies whether DIAdem cancels the measurement when an OPC block does not receive any values over a certain period of time."
---

# OPCSetErrAction

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetErrAction

Specifies whether DIAdem cancels the measurement when an OPC block does not receive any values over a certain period of time.

## Signature

```python
dd.OPCSetErrAction(OPCErrAction)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCErrAction</td>
<td>Specifies whether DIAdem cancels a measurement during a timeout to OPC servers.<div id="exp_OPCErrAction">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCErrAction &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCErrAction</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid" width="400"><strong>OPC Input</strong></td>
<td style="BORDER-BOTTOM: 1px solid" width="400"><strong>OPC Output</strong></td>
</tr>
<tr>
<td width="150">0</td>
<td width="400">DIAdem cancels the measurement.</td>
<td width="400">DIAdem cancels the measurement.</td>
</tr>
<tr>
<td width="150">1</td>
<td width="400">DIAdem continues the measurement and replaces the missing measurement values with NoValues.</td>
<td width="400">DIAdem continues the measurement and replaces the missing measurement values with NoValues.</td>
</tr>
<tr>
<td width="150">2</td>
<td width="400">DIAdem continues the measurement and replaces the missing measurement values with the last acquired value.</td>
<td width="400"> </td>
</tr>
</table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetErrAction.htm`*

---
title: "OPCSetCallTo"
description: "Restricts the period for unconfirmed OPC operations."
---

# OPCSetCallTo

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetCallTo

Restricts the period for unconfirmed OPC operations.

## Signature

```python
dd.OPCSetCallTo(OPCCallTO)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCCallTO</td>
<td>Specifies the time in milliseconds after which DIAdem terminates unconfirmed OPC operations.<div id="exp_OPCCallTO">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCCallTo &lt;= 600000</td></tr>
</table> The default value is 5000 milliseconds.<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetCallTo.htm`*

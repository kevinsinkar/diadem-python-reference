---
title: "OPCSetConnectTo"
description: "Restricts the period for the link-up to OPC servers."
---

# OPCSetConnectTo

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetConnectTo

Restricts the period for the link-up to OPC servers.

## Signature

```python
dd.OPCSetConnectTo(OPCConnectTO)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCConnectTO</td>
<td>Specifies the time in milliseconds after which DIAdem disconnects a link to an OPC server.<div id="exp_OPCConnectTO">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCConnectTo &lt;= 600000</td></tr>
</table>The default value is 15000 milliseconds.<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetConnectTo.htm`*

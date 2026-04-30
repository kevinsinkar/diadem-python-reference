---
title: "OPCGetAutoValid"
description: "Determines how DIAdem validates OPC items."
---

# OPCGetAutoValid

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCGetAutoValid

Determines how DIAdem validates OPC items.

## Signature

```python
dd.OPCGetAutoValid()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless" id="table2">
<tr><td width="150">OPCAutoValid</td>
<td>Specifies whether DIAdem runs a request before validating OPC items.<div id="exp_OPCAutoValid">
<table class="Borderless" id="table3">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCAutoValid &lt;= 1</td></tr>
</table>
<p>The <span class="Monospace">OPCAutoValid</span> variable can contain the following values:</p>
<table class="Borderless" id="table4">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr><td width="150">0</td><td>A request occurs before validation.</td></tr><tr><td width="150">1</td><td>The validation runs directly and without a confirmation prompt.</td></tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCGetAutoValid.htm`*

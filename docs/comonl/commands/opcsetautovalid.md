---
title: "OPCSetAutoValid"
description: "Validates OPC items."
---

# OPCSetAutoValid

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetAutoValid

Validates OPC items.

## Signature

```python
dd.OPCSetAutoValid(OPCAutoValid)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCAutoValid</td>
<td>Specifies whether DIAdem runs a request before validating OPC items.<div id="exp_OPCAutoValid">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCAutoValID &lt;= 1</td></tr>
</table>
<p>The <span class="Monospace">OPCAutoValid</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>A request occurs before validation.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>The validation runs directly and without a confirmation prompt.</td></tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetAutoValid.htm`*

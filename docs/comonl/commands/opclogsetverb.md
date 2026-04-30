---
title: "OPCLogSetVerb"
description: "Specifies the settings of the logfile for OPC communication."
---

# OPCLogSetVerb

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCLogSetVerb

Specifies the settings of the logfile for OPC communication.

## Signature

```python
dd.OPCLogSetVerb(OPCLogCategory, OPCLogEnableCat)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCLogCategory</td>
<td>Specifies which categories DIAdem records in an OPC logfile.<div id="exp_OPCLogCategory">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCLogCategory &lt;= 3</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCLogCategory</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>DIAdem records error messages.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>DIAdem records warning messages.</td></tr><tr><td width="150"><pre><donottranslate>2</donottranslate></pre></td><td>DIAdem records general information.</td></tr><tr><td width="150"><pre><donottranslate>3</donottranslate></pre></td><td>DIAdem records information about the measurement preparation.</td></tr></table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCLogEnableCat</td>
<td>Specifies whether DIAdem records the categories listed in the <span class="Monospace">OPCLogCategory</span> variables.<div id="exp_OPCLogEnableCat">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCLogEnableCat &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCLogEnableCat</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>DIAdem does not record the category in the OPC logfile.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>DIAdem records the category in the OPC logfile.</td></tr></table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCLogSetVerb.htm`*

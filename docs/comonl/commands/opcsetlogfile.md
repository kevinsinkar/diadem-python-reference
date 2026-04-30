---
title: "OPCSetLogFile"
description: "Specifies whether DIAdem records the OPC communication in a logfile."
---

# OPCSetLogFile

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetLogFile

Specifies whether DIAdem records the OPC communication in a logfile.

## Signature

```python
dd.OPCSetLogFile(OPCEnableLog, OPCLogName, OPCLogReset)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCEnableLog</td>
<td>Specifies whether DIAdem records the OPC communication in a logfile.<div id="exp_OPCEnableLog">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCEnableLog &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCEnableLog</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>DIAdem does not write a logfile.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>DIAdem writes a logfile.</td></tr></table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCLogName</td>
<td>Specifies the name of the logfile for recording the OPC communication.<div id="exp_OPCLogName">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OPCLogReset</td>
<td>Specifies when DIAdem creates a new logfile.<div id="exp_OPCLogReset">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCLogReset &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCLogReset</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>DIAdem creates a new logfile when the program starts.</td>
</tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>DIAdem creates a new logfile when the measurement starts.</td>
</tr><tr><td width="150"><pre><donottranslate>2</donottranslate></pre></td><td>DIAdem creates a new logfile when prompted by the user.</td>
</tr></table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetLogFile.htm`*

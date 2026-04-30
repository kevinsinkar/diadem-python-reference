---
title: "OPCGetLogFile"
description: "Determines whether DIAdem records the OPC communication in a logfile."
---

# OPCGetLogFile

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCGetLogFile

Determines whether DIAdem records the OPC communication in a logfile.

## Signature

```python
dd.OPCGetLogFile()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150">OPCEnableLog</td><td>Receives information as to whether DIAdem records the OPC communication in a logfile.<div id="exp_OPCEnableLog__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCEnableLog &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCEnableLog</span> variable can contain the following values:</p>
<table class="Borderless" id="table1">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr><td width="150">0</td><td>DIAdem does not write a logfile.</td></tr><tr><td width="150">1</td><td>DIAdem writes a logfile.</td></tr></table>
<p class="Body">
</p></div></td></tr><tr><td width="150">OPCLogName</td><td>Receives the name of the logfile for recording the OPC communication.<div id="exp_OPCLogName__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
</div></td></tr><tr><td width="150">OPCLogReset</td><td>Receives information as to when DIAdem creates a logfile.<div id="exp_OPCLogReset__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCLogReset &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCLogReset</span> variable can contain the following values:</p>
<table class="Borderless" id="table2">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr>
<td width="150">0</td><td>DIAdem creates a new logfile when the program launches.</td>
</tr>
<tr>
<td width="150">1</td><td>DIAdem creates a new logfile when the measurement starts.</td>
</tr>
<tr>
<td width="150">2</td><td>DIAdem creates a new logfile on request.</td>
</tr>
</table>
</div></td></tr></table>
</div>

---

*Source: `ComOnl/OPCGetLogFile.htm`*

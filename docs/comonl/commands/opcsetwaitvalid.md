---
title: "OPCSetWaitValid"
description: "Specifies whether, and how long, DIAdem waits until the OPC block receives valid measured values from the OPC server."
---

# OPCSetWaitValid

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetWaitValid

Specifies whether, and how long, DIAdem waits until the OPC block receives valid measured values from the OPC server.

## Signature

```python
dd.OPCSetWaitValid(OPCWaitValid, OPCTOWaitValid)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table21"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>If the OPC block does not receive any valid measurement values from the OPC server within the period of time specified by the <span class="Monospace">OPCTOWaitValid</span> variable, DIAdem executes the action that is specified in the <a href="../opcseterraction/">OPCSetErrAction</a>.</td></tr></table>
<table class="Borderless" id="table22">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetWaitValid(<em>Value1,Value2</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCWaitValid</td>
<td>Specifies whether DIAdem waits for valid values from the OPC server, after the start of a measurement.<div id="exp_OPCWaitValid">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCWaitValid &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCWaitValid</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr>
<td width="150"><pre><donottranslate>0</donottranslate></pre>
</td><td>DIAdem starts the measurement without waiting for valid measurement values from an OPC server.</td>
</tr>
<tr>
<td width="150"><pre><donottranslate>1</donottranslate></pre>
</td><td>After the measurement starts, DIAdem waits until all measurement points of the OPC block receive valid values from the OPC server.</td>
</tr>
</table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCTOWaitValid</td>
<td>Specifies the time in milliseconds that DIAdem waits for valid values from the OPC server, after the start of the measurement.<div id="exp_OPCTOWaitValid">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCTOWaitValid &lt;= 1000000</td></tr>
</table>
</div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetWaitValid.htm`*

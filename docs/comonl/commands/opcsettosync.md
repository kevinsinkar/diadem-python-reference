---
title: "OPCSetToSync"
description: "Limits the period of time that an OPC server may wait for the response to asynchronous calls."
---

# OPCSetToSync

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetToSync

Limits the period of time that an OPC server may wait for the response to asynchronous calls.

## Signature

```python
dd.OPCSetToSync(OPCTOSync)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table16">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetTOSync(<em>Timeout</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCTOSync</td>
<td>Specifies the time in milliseconds after which DIAdem interrupts synchronous calls to an OPC server.<div id="exp_OPCTOSync">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCToSync &lt;= 1000000</td></tr>
</table>Use the <a href="../opcseterraction/">OPCSetErrAction</a> command to specify the reaction to timeouts.<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetToSync.htm`*

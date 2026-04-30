---
title: "OPCSetChkAS"
description: "Checks asynchronous connections of an OPC block to the OPC server."
---

# OPCSetChkAS

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetChkAS

Checks asynchronous connections of an OPC block to the OPC server.

## Signature

```python
dd.OPCSetChkAS(OPCChkAs, OPCChkAsIntrv)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table7"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note  </strong>The <span class="Monospace">OPCSetChkAs</span> command can only check the connection to the OPC server if you have set asynchronous mode for the OPC block.</td></tr></table>
<table class="Borderless" id="table8">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/><br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCSetChkAs(<em>1,Interval</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCChkAs</td>
<td>Specifies whether DIAdem checks asynchronous connections to OPC servers during the measurement.<div id="exp_OPCChkAs">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCChkAs &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCChkAs</span> variable can contain the following values:</p>
<table class="Borderless">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>0</donottranslate></pre></td><td>DIAdem does not check asynchronous connections.</td></tr><tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>DIAdem checks asynchronous connections.</td></tr></table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCChkAsIntrv</td>
<td>Specifies the number of clock cycles after which DIAdem checks asynchronous connections to OPC servers again.<div id="exp_OPCChkAsIntrv">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCChkAsIntrV &lt;= 2147483647</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
</table>
</div>

---

*Source: `ComOnl/OPCSetChkAS.htm`*

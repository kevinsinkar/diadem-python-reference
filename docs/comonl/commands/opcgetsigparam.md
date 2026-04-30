---
title: "OPCGetSigParam"
description: "Determines the parameters for an OPC signal."
---

# OPCGetSigParam

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCGetSigParam

Determines the parameters for an OPC signal.

## Signature

```python
dd.OPCGetSigParam(OPCSigIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table15">
<tr>
<td class="Icon"><img src="image/note.gif"/></td>
<td><strong>Note  </strong>You must use the following object hierarchy to execute this command:<br attr="ext"/>
 <br attr="ext"/>
<pre><donottranslate>Call DACObjOpen(<em>BlockName</em>)<br attr="ext"/>    Call OPCGetSigParam(<em>OPCSignalIndex</em>)<br attr="ext"/>Call DACObjClose(<em>BlockName</em>)</donottranslate></pre>
<br attr="ext"/>You need the DAC block name to open the DAC block, to execute the command, and to close the DAC block.<br attr="ext"/>
<br attr="ext"/>Refer to <a href="#" data-unresolved="1">Accessing Objects in DIAdem DAC</a> for more information.</td>
</tr>
</table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCSigIndex</td>
<td>Specifies the index of a signal in an OPC block.<div id="exp_OPCSigIndex">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCSigIndex &lt;= 2147483647</td></tr>
</table>
<p>The index starts with <span class="Monospace">1</span>.</p>
</div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr>
<td width="150">OPCSigName</td>
<td>Receives the name of a signal in an OPC block.<div id="exp_OPCSigName">
<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">String variable</a></td>
</tr>
<tr>
<td>Maximum 80 characters</td>
</tr>
</table>
</div>
</td>
</tr>
<tr>
<td width="150">OPCItemID</td>
<td>Receives the ID of an OPC item.<div id="exp_OPCItemID">
<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">String variable</a></td>
</tr>
<tr>
<td>Maximum 80 characters</td>
</tr>
</table>
<p class="Body"></p>
</div>
</td>
</tr>
<tr>
<td width="150">OPCActiveFlag</td>
<td>Receives information as to whether a signal of an OPC block is active.<div id="exp_OPCActiveFlag">
<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Longinteger variable</a></td>
</tr>
<tr>
<td>0 &lt;= OPCActiveFlag &lt;= 1</td>
</tr>
</table>
<p class="body">The OPCActiveFlag variable can contain the following values:</p>
<table class="Borderless" id="table1">
<tr>
<td width="150"><strong>Value</strong></td>
<td><strong>Meaning</strong></td>
</tr>
<tr>
<td width="150">0</td>
<td>The OPC signal is not active.</td>
</tr>
<tr>
<td width="150">1</td>
<td>The OPC signal is active.</td>
</tr>
</table>
<p> </p>
</div>
</td>
</tr>
<tr>
<td width="150">OPCArrayEnable</td>
<td>Receives information as to whether array indexing is executed for a signal in an OPC block.<div id="exp_OPCArrayEnable">
<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Longinteger variable</a></td>
</tr>
<tr>
<td>0 &lt;= OPCArrayEnable &lt;= 1</td>
</tr>
</table>
<p class="Body">The <span class="Monospace">OPCArrayEnable</span> variable can contain the following values:</p>
<table class="Borderless" id="table2">
<tr>
<td width="150"><strong>Value</strong></td>
<td><strong>Meaning</strong></td>
</tr>
<tr>
<td width="150">0</td>
<td>No array indexing for signal.</td>
</tr>
<tr>
<td width="150">1</td>
<td>Array indexing for signal.</td>
</tr>
</table>
<p class="Body"></p>
</div>
</td>
</tr>
<tr>
<td width="150">OPCArrayIndex</td>
<td>Receives the index of the value that is to be read, when the OPC server returns an array for the OPC item.<div id="exp_OPCArrayIndex">
<table class="Borderless">
<tr>
<td><a href="#" data-unresolved="1">Longinteger variable</a></td>
</tr>
<tr>
</tr>
</table>
<p class="Body">The array length limits the value range.</p>
<p class="Body"></p>
</div>
</td>
</tr>
</table>
</div>

## Python example

```python
dd.DACObjOpen("OPC-Input")
OPCGetSigParam(2)
dd.DACObjClose("OPC-Input")
print(OPCSigName,0,"OPCSigName")
print(OPCItemID,0,"OPCItemID")
print(OPCActiveFlag,0,"OPCActiveFlag")
print(OPCArrayEnable,0,"OPCArrayEnable")
print(OPCArrayIndex,0,"OPCArrayIndex")
```

---

*Source: `ComOnl/OPCGetSigParam.htm`*

---
title: "OPCGetBlockParam"
description: "Determines the settings of an OPC block in the block diagram."
---

# OPCGetBlockParam

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCGetBlockParam

Determines the settings of an OPC block in the block diagram.

## Signature

```python
dd.OPCGetBlockParam()
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td>None</td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCMode</td><td>Receives the communication mode between the OPC block and an OPC server.<div id="exp_OPCMode">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCMode &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCMode</span> variable can contain the following values:</p>
<table class="Borderless" id="table1">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr><td width="150">0</td><td>The communication is synchronous.</td></tr><tr><td width="150">1</td><td>The communication is asynchronous.</td></tr></table>
</div></td></tr>
<tr><td width="150">OPCUpdRate</td><td>Receives the time in milliseconds after which an OPC server regularly updates the data in an OPC group.<div id="exp_OPCUpdRate">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr>
<tr><td width="150">OPCDeadband</td><td>Receives the deadband as a percentage.<div id="exp_OPCDeadband">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Floating-point number variable</a></td></tr>
<tr>
<td>0 &lt;= OPCDeadBand &lt;= 100</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OPCDeviceRead</td><td>Receives the type of read access for an OPC block.<div id="exp_OPCDeviceRead">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCDeviceRead &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCDeviceRead</span> variable can contain the following values:</p>
<table class="Borderless" id="table7">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr><td width="150">0</td><td>The OPC block contains the values in a buffer.</td>
</tr><tr><td width="150">1</td><td>The OPC block reads the values directly from the OPC signals.</td>
</tr></table>
<p class="Body"> </p>
</div></td></tr>
<tr><td width="150">OPCWaitValid</td><td>Receives information as to whether DIAdem waits for valid values from the OPC server, after the start of a measurement.<div id="exp_OPCWaitValid">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCWaitValid &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCWaitValid</span> variable can contain the following values:</p>
<table class="Borderless" id="table2">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr><td width="151">0</td><td width="720">DIAdem starts the measurement without waiting for valid measurement values from an OPC server.</td></tr><tr><td width="151">1</td><td width="720">After the measurement starts, DIAdem waits until all measurement points of the OPC block receive valid values from the OPC server.</td></tr></table>
</div></td></tr>
<tr><td width="150">OPCTOWaitValid</td><td>Receives the time in milliseconds that DIAdem waits for valid values from the OPC server, after the start of the measurement.<div id="exp_OPCTOWaitValid">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCTOWaitValid &lt;= 1000000</td></tr>
</table>
</div></td></tr>
<tr><td width="150">OPCTOSync</td><td>Receives the time in milliseconds after which DIAdem interrupts synchronous calls to OPC servers. Use the <a href="../opcseterraction/">OPCSetErrAction</a> command to specify the reaction to timeouts.<div id="exp_OPCTOSync">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCToSync &lt;= 1000000</td></tr>
</table>
</div></td></tr><tr>
<td width="150">OPCErrAction</td>
<td>Receives information as to whether DIAdem cancels a measurement during a timeout to OPC servers.<div id="exp_OPCErrAction">
<table class="Borderless" id="table4">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCErrAction &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCErrAction</span> variable can contain the following values:</p>
<table class="Borderless" id="table5">
<tr>
<td width="150"><strong>Value</strong></td>
<td width="400"><strong>OPC Input</strong></td>
<td width="400"><strong>OPC Output</strong></td>
</tr>
<tr>
<td width="150">0</td>
<td width="400">Cancels the measurement.</td>
<td width="400">Cancels the measurement.</td>
</tr>
<tr>
<td width="150">1</td>
<td width="400">Continues the measurement and uses NoValues for the missing measured values.</td>
<td width="400">Continues the measurement without outputting other values to the OPC server.</td>
</tr>
<tr>
<td width="150">2</td>
<td width="400">Continues the measurement and uses the last acquired value for the missing measured values.</td>
<td width="400"> </td>
</tr>
</table>
</div></td></tr><tr><td width="150">OPCChkAs</td><td>Receives information as to whether DIAdem checks asynchronous connections during the measurement.<div id="exp_OPCChkAs__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCChkAs &lt;= 1</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCChkAs</span> variable can contain the following values:</p>
<table class="Borderless" id="table6">
<tr>
<td width="150"><strong>Value</strong></td><td><strong>Meaning</strong></td>
</tr>
<tr><td width="150">0</td><td width="721">DIAdem does not check asynchronous connections.</td></tr><tr><td width="150">1</td><td width="721">DIAdem checks asynchronous connections.</td></tr></table>
</div></td></tr><tr><td width="150">OPCChkAsIntrv</td><td>Receives the information as to the number of clock cycles after which DIAdem checks asynchronous connections to OPC servers.<div id="exp_OPCChkAsIntrv__1">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
</tr>
</table>
</div></td></tr></table>
</div>

## Python example

```python
dd.DACObjOpen("OPC-Input")
OPCGetBlockParam()
dd.DACObjClose("OPC-Input")

print(OPCMode,0,"OPCMode")
print(OPCUpdRate,0,"OPCUpdRate")
print(OPCDeadband,0,"OPCDeadband")
print(OPCDeviceRead,0,"OPCDeviceRead")
print(OPCWaitValid,0,"OPCWaitValid")
print(OPCTOWaitValid,0,"OPCTOWaitValid")
print(OPCTOSync,0,"OPCTOSync")
print(OPCChkAs,0,"OPCChkAs")
print(OPCChkAsIntrv,0,"OPCChkAsIntrv")
print(OPCErrAction,0,"OPCErrAction")
```

---

*Source: `ComOnl/OPCGetBlockParam.htm`*

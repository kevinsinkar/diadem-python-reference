---
title: "OPCReadSync"
description: "Reads values from items of an OPC group"
---

# OPCReadSync

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCReadSync

Reads values from items of an OPC group

## Signature

```python
dd.OPCReadSync(OPCGrpHandle, OPCItemNo, OPCDataSource)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table14"><tr><td class="Icon"><img height="25" src="image/note.gif" width="26"/></td><td><strong>Note</strong>  After the <span class="Monospace">OPCReadSync</span> command has read the OPC items, the variables <a href="../opcgetint/">OPCGetInt</a>, <a href="../opcgetdouble/">OPCGetDouble</a>, and <a href="../opcgetstring/">OPCGetString</a> contain the read values.</td></tr></table>
</div>

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCGrpHandle</td>
<td>Specifies the handle of an OPC group.<div id="exp_OPCGrpHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCGrpHandle &lt;= 2147483647</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCItemNo</td>
<td>Specifies the number of items of an OPC group that are to be processed.<div id="exp_OPCItemNo">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCItemNo &lt;= 2147483647</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCDataSource</td>
<td>Specifies whether DIAdem reads the values from a buffer or directly from the measurement point.<div id="exp_OPCDataSource">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>1 &lt;= OPCDataSource &lt;= 2</td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCDataSource</span> variable can contain the following values:</p>
<table class="Borderless" id="table1">
<tr>
<td style="BORDER-BOTTOM: 1px solid" width="150"><strong>Value</strong></td>
<td style="BORDER-BOTTOM: 1px solid"><strong>Meaning</strong></td>
</tr>
<tr><td width="150"><pre><donottranslate>1</donottranslate></pre></td><td>The OPC server holds the values in a buffer.</td>
</tr><tr><td width="150"><pre><donottranslate>2</donottranslate></pre></td><td>DIAdem receives the values directly from the measurement point of the OPC server.</td>
</tr></table>
<p>
</p></div></td></tr>
</table>
</div>

## Returns

<div markdown="1">
<table class="Borderless"><tr><td width="150">OPCErrorCode</td><td>Receives the status of the OPC command.<div id="exp_OPCErrorCode">
<table class="Borderless" id="table8">
<tr>
<td><a href="#" data-unresolved="1">Longinteger variable</a></td>
</tr>
<tr>
<td>0 &lt;= OPCErrorCode &lt;= 2147483647</td>
</tr>
</table>
<p class="Body">The <span class="Monospace">OPCErrorCode</span> variable returns the number or the OPC code of the respective message:</p>
<table class="Borderless" id="table9">
<tr>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="50"><strong>No.</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="220"><strong>OPC code</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="220"><strong>Description</strong></td>
</tr>
<tr>
<td width="50">0</td>
<td>eOPCAuto_Ok</td>
<td>DIAdem executed the command without errors.</td>
</tr>
<tr>
<td width="50">1</td>
<td>eOPCAuto_GeneralError</td>
<td>A global error has occurred.</td>
</tr>
<tr>
<td width="50">2</td>
<td>eOPCAuto_BlockMapEntryNotFound</td>
<td>DIAdem cannot find entry for the signal and device specification in the driver blockmap.</td>
</tr>
<tr>
<td width="50">3</td>
<td>eOPCAuto_UnidentifiedBlocktype</td>
<td>The block type is not valid because no DAC input block or DAC output block open.</td>
</tr>
<tr>
<td width="50">4</td>
<td>eOPCAuto_OPCBlockNotOpen</td>
<td>No DAC block opened with the <a href="../dacobjopen/">DACObjOpen</a> command.</td>
</tr>
<tr>
<td width="50">5</td>
<td>eOPCAuto_InvalidSignalIndex</td>
<td>The signal index is not valid. Values from <span class="Monospace">1</span> to <span class="Monospace">255</span> are valid.</td>
</tr>
<tr>
<td width="50">6</td>
<td>eOPCAuto_InvalidLogReset</td>
<td>The value for the time of the logfile reset is not valid.</td>
</tr>
<tr>
<td width="50">7</td>
<td>eOPCAuto_InvalidReportVerbosity</td>
<td>The value for the type and extent of information to be recorded is not valid.</td>
</tr>
<tr>
<td width="50">8</td>
<td>eOPCAuto_ProgIDNotInLocalRegistry</td>
<td>DIAdem cannot find the transferred ProgID in the local registration.</td>
</tr>
<tr>
<td width="50">9</td>
<td>eOPCAuto_ServerNotConnected</td>
<td>The OPC server is not connected.</td>
</tr>
<tr>
<td width="50">10</td>
<td>eOPCAuto_DataConversionFail</td>
<td>Data could not be converted.</td>
</tr>
<tr>
<td width="50">11</td>
<td>eOPCAuto_InvalidErrorAction</td>
<td>The value provided for the error reaction is invalid.</td>
</tr>
<tr>
<td width="50">12</td>
<td>eOPCAuto_InvalidDACSigListLen</td>
<td>The length of the DAC signal list specified in the block is invalid.</td>
</tr>
<tr>
<td width="50">13</td>
<td>eOPCAuto_InvalidServerName</td>
<td>The name of the OPC server is invalid.</td>
</tr>
<tr>
<td width="50">14</td>
<td>eOPCAuto_NotImplemented</td>
<td>The function is not implemented.</td>
</tr>
<tr>
<td width="50">15</td>
<td>eOPCAuto_RemoteConnectWithoutClassID</td>
<td>Transfer the ClassID to the OPCSrvConnect command to access a remote server without local registration. You only can reference OPC servers on remote computers with the ProgID if the ProgID or the server are registered locally.</td>
</tr>
<tr>
<td width="50">16</td>
<td>eOPCAuto_ArrayAccesNotAllowed</td>
<td>The function cannot access arrays.</td>
</tr>
<tr>
<td width="50">17</td>
<td>eOPCAuto_NoMoreHandles</td>
<td>No more OPC objects possible in the script area.</td>
</tr>
<tr>
<td width="50">18</td>
<td>eOPCAuto_InvalidServerHandle</td>
<td>The server handle is invalid.</td>
</tr>
<tr>
<td width="50">19</td>
<td>eOPCAuto_InvalidGroupHandle</td>
<td>The group handle is invalid.</td>
</tr>
<tr>
<td width="50">20</td>
<td>eOPCAuto_InvalidItemHandle</td>
<td>The item handle is invalid.</td>
</tr>
<tr>
<td width="50">21</td>
<td>eOPCAuto_ConnectTimeout</td>
<td>Timeout occurred while connecting to OPC server. The server cannot be accessed or one of the Proxy-DLLs such as <span class="Monospace">opcproxy.dll</span> and <span class="Monospace">opccomn_ps.dll</span>, is not registered.</td>
</tr>
<tr>
<td width="50">22</td>
<td>eOPCAuto_CallTimeout</td>
<td>A timeout occurred while a function on an OPC server was being called.</td>
</tr>
<tr>
<td width="50">23</td>
<td>eOPCAuto_NoIOPCServer</td>
<td>No IOPCServer interface at OPC server.</td>
</tr>
<tr>
<td width="50">24</td>
<td>eOPCAuto_NoIOPCItemMgt</td>
<td>No IOPCItemMgt interface at OPC server.</td>
</tr>
<tr>
<td width="50">25</td>
<td>eOPCAuto_NoIOPCSyncIO</td>
<td>No IOPCSyncIO interface at OPC server.</td>
</tr>
<tr>
<td width="50">26</td>
<td>eOPCAuto_NoIOPCGroupStateMgt</td>
<td>No IOPCGroupStateMgt interface at OPC server.</td>
</tr>
<tr>
<td width="50">27</td>
<td>eOPCAuto_InvalidItemNo</td>
<td>The number of items is invalid or an OPC group contains more items than acceptable.</td>
</tr>
</table>
</div>
</td></tr><tr><td width="150">OPCHResult</td><td>Receives the return value of the OPC command.<div id="exp_OPCHResult">
<table class="Borderless" id="table11">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
</table>
<p class="Body">The <span class="Monospace">OPCHResult</span> variable can contain the following values:</p>
<table class="Borderless" id="table12">
<tr>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="50"><strong>Value</strong></td>
<td style="border-bottom-style: solid; border-bottom-width: 1" width="220"><strong>Meaning</strong></td>
</tr>
<tr>
<td width="150">0</td>
<td>The command was executed successfully.</td>
</tr>
<tr>
<td width="150">1</td>
<td>The command was only partially executed successfully. The <a href="../../../varonl/variables/aopcitemerror/">aOPCItemError</a> variable contains information.</td>
</tr>
</table>
</div>
</td></tr><tr><td width="150">aOPCItemError</td><td>Receives the status of operations with various OPC items.<div id="exp_aOPCItemError">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a><br attr="ext"/>i = 1 ... 1024</td></tr>
<tr>
</tr>
</table>
<p class="Body">Specify the field length with the <a href="../../../varonl/variables/opcitemno/">OPCItemNo</a> variable.</p><p class="Body">The <span class="Monospace">aOPCItemError</span> variable can contain the following values:</p><table class="Borderless" id="table13">
<tr>
<td width="50"><strong>Value</strong></td>
<td width="220"><strong>Meaning</strong></td>
</tr>
<tr><td width="150">0</td><td>Command executed successfully.</td></tr><tr><td width="150">Other</td><td>Command could not execute. The <a href="../../../varonl/variables/opcerrorcode/">OPCErrorCode</a> variable contains a list of error codes.</td></tr></table>
<p class="Body">
</p></div></td></tr></table>
</div>

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eOPCAuto_Ok` | 0 | DIAdem executed the command without errors. |
| `eOPCAuto_GeneralError` | 1 | A global error has occurred. |
| `eOPCAuto_BlockMapEntryNotFound` | 2 | DIAdem cannot find entry for the signal and device specification in the driver blockmap. |
| `eOPCAuto_UnidentifiedBlocktype` | 3 | The block type is not valid because no DAC input block or DAC output block open. |
| `eOPCAuto_OPCBlockNotOpen` | 4 | No DAC block opened with the DACObjOpen command. |
| `eOPCAuto_InvalidSignalIndex` | 5 | The signal index is not valid. Values from 1 to 255 are valid. |
| `eOPCAuto_InvalidLogReset` | 6 | The value for the time of the logfile reset is not valid. |
| `eOPCAuto_InvalidReportVerbosity` | 7 | The value for the type and extent of information to be recorded is not valid. |
| `eOPCAuto_ProgIDNotInLocalRegistry` | 8 | DIAdem cannot find the transferred ProgID in the local registration. |
| `eOPCAuto_ServerNotConnected` | 9 | The OPC server is not connected. |
| `eOPCAuto_DataConversionFail` | 10 | Data could not be converted. |
| `eOPCAuto_InvalidErrorAction` | 11 | The value provided for the error reaction is invalid. |
| `eOPCAuto_InvalidDACSigListLen` | 12 | The length of the DAC signal list specified in the block is invalid. |
| `eOPCAuto_InvalidServerName` | 13 | The name of the OPC server is invalid. |
| `eOPCAuto_NotImplemented` | 14 | The function is not implemented. |
| `eOPCAuto_RemoteConnectWithoutClassID` | 15 | Transfer the ClassID to the OPCSrvConnect command to access a remote server without local registration. You only can reference OPC servers on remote computers with the ProgID if the ProgID or the server are registered locally. |
| `eOPCAuto_ArrayAccesNotAllowed` | 16 | The function cannot access arrays. |
| `eOPCAuto_NoMoreHandles` | 17 | No more OPC objects possible in the script area. |
| `eOPCAuto_InvalidServerHandle` | 18 | The server handle is invalid. |
| `eOPCAuto_InvalidGroupHandle` | 19 | The group handle is invalid. |
| `eOPCAuto_InvalidItemHandle` | 20 | The item handle is invalid. |
| `eOPCAuto_ConnectTimeout` | 21 | Timeout occurred while connecting to OPC server. The server cannot be accessed or one of the Proxy-DLLs such as opcproxy.dll and opccomn_ps.dll , is not registered. |
| `eOPCAuto_CallTimeout` | 22 | A timeout occurred while a function on an OPC server was being called. |
| `eOPCAuto_NoIOPCServer` | 23 | No IOPCServer interface at OPC server. |
| `eOPCAuto_NoIOPCItemMgt` | 24 | No IOPCItemMgt interface at OPC server. |
| `eOPCAuto_NoIOPCSyncIO` | 25 | No IOPCSyncIO interface at OPC server. |
| `eOPCAuto_NoIOPCGroupStateMgt` | 26 | No IOPCGroupStateMgt interface at OPC server. |
| `eOPCAuto_InvalidItemNo` | 27 | The number of items is invalid or an OPC group contains more items than acceptable. |

---

*Source: `ComOnl/OPCReadSync.htm`*

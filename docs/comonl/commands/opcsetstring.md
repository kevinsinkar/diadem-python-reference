---
title: "OPCSetString"
description: "Assigns a String type value to an OPC server."
---

# OPCSetString

!!! abstract "Command &middot; `ComOnl.chm`"
    Command: OPCSetString

Assigns a String type value to an OPC server.

## Signature

```python
dd.OPCSetString(OPCItemHandle, OPCStringValue)
```

## Parameters

<div markdown="1">
<table class="Borderless">
<tr><td width="150">OPCItemHandle</td>
<td>Specifies the handle of an OPC item.<div id="exp_OPCItemHandle">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">Longinteger variable</a></td></tr>
<tr>
<td>0 &lt;= OPCItemHandle &lt;= 2147483647</td></tr>
</table>
<p class="Body">
</p></div></td></tr>
<tr><td width="150">OPCStringValue</td>
<td>Specifies the current value of an OPC item.<div id="exp_OPCStringValue">
<table class="Borderless">
<tr><td><a href="#" data-unresolved="1">String variable</a></td></tr>
<tr>
<td>Maximum 80 characters</td></tr>
</table>
</div></td></tr>
</table>
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

*Source: `ComOnl/OPCSetString.htm`*

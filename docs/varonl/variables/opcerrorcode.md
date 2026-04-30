---
title: "OPCErrorCode"
description: "Contains the status of the OPC command."
---

# OPCErrorCode

!!! abstract "Variable &middot; `VarOnl.chm`"
    Variable: OPCErrorCode

Contains the status of the OPC command.

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
| `eOPCAuto_RemoteConnectWithoutClassID` | 15 | Transfer the ClassID to the OPCSrvConnect command to access a remote server without local registration. To access an OPC server on another computer you must specify the ProgID. |
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

*Source: `VarOnl/OPCErrorCode.htm`*

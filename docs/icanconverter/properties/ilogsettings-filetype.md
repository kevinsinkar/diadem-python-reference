---
title: "ILogSettings.FileType"
description: "Specifies in the Bus Log Converter the file type of the logfile to be converted. The file type eLogFileTypeTTL is a preview feature and can only be used in the "
---

# ILogSettings.FileType

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: FileType for LogSettings

Specifies in the Bus Log Converter the file type of the logfile to be converted. The file type eLogFileTypeTTL is a preview feature and can only be used in the Bus Log Converter if you have enabled the corresponding preview feature. Preview features are new developments that will be available as a full feature in one of the upcoming DIAdem versions. The user interface, the API, and the scope of functions is subject to change.

## Signature

```python
obj.FileType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLogFileTypeNI` | 1 | NI-CAN |
| `eLogFileTypeGIN` | 2 | GIN |
| `eLogFileTypeVBLF` | 3 | Vector BLF |
| `eLogFileTypeVLOG` | 4 | Vector LOG |
| `eLogFileTypeVASC` | 5 | Vector ASCII |
| `eLogFileTypeILOG` | 6 | Ipetronik MLOG/SLOG |
| `eLogFileTypePCAN` | 7 | PCAN Trace |
| `eLogFileTypeTdms` | 8 | NI XNET (TDMS) |
| `eLogFileTypeKLOG` | 9 | KVASER LOG |
| `eLogFileTypeIOS` | 10 | IOSiX IOS |
| `eLogFileTypeSIE` | 11 | SoMat SIE |
| `eLogFileTypeMDF4` | 12 | ASAM MDF4 |
| `eLogFileTypeTELEMACO` | 13 | Telemaco |
| `eLogFileTypeKASC` | 14 | KVASER ASCII |
| `eLogFileTypeHEAD` | 15 | Head HDF |
| `eLogFileTypeHYDAC` | 16 | Hydac BIN |
| `eLogFileTypeIXXAT` | 17 | IXXAT CSV |
| `eLogFileTypeTTL` | 19 | TTTech TTL Processes only CAN, LIN, and FlexRay frames. |

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.LogSettings.FileType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_FileType_ILogSettings.htm`*

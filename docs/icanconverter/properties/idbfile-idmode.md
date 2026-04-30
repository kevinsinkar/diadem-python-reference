---
title: "IDbFile.IdMode"
description: "Specifies in the Bus Log Converter whether the database file is a standard file or a file with a special mode."
---

# IDbFile.IdMode

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: IdMode for DbFile

Specifies in the Bus Log Converter whether the database file is a standard file or a file with a special mode.

## Signature

```python
obj.IdMode
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDbFileIdModeDEFAULT` | 1 | Standard file |
| `eDbFileIdModeJ1939` | 2 | File with the mode J1939 If you use this mode, DIAdem interprets the last byte of the ID as the source address and uses the integer number between 0 and 255 as the CAN source address in the group properties. An underscore and this integer number is added to the group name. |
| `eDbFileIdModeNMea2000` | 3 | File with the NMEA2000 mode. This mode is standard for serial data networking of electronic devices in naval vessels and is also frequently used by GPS hardware on commercial vehicles or agricultural machinery. For more information, visit the National Marine Electronics Association website. |

## Python example

```python
oMyDbFile = dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles(1)
print(oMyDbFile.IdMode)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_IdMode_IDbFile.htm`*

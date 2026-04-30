---
title: "IDbFile.File"
description: "Specifies the name and the path of a database file that is associated with a specific bus in the Bus Log Converter ."
---

# IDbFile.File

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: File for DbFile

Specifies the name and the path of a database file that is associated with a specific bus in the Bus Log Converter .

## Signature

```python
obj.File
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles(1).File)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_File_IDbFile.htm`*

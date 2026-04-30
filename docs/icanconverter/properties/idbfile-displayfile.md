---
title: "IDbFile.DisplayFile"
description: "Specifies in the Bus Log Converter the name of a database file that belongs to a specific bus. The DisplayFile property is write-protected and does not contain "
---

# IDbFile.DisplayFile

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: DisplayFile for DbFile

Specifies in the Bus Log Converter the name of a database file that belongs to a specific bus. The DisplayFile property is write-protected and does not contain the file path.

## Signature

```python
obj.DisplayFile
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles(1).DisplayFile)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_DisplayFile_IDbFile.htm`*

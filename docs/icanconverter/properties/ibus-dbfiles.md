---
title: "IBus.DbFiles"
description: "Returns the database files that are associated with a bus in the Bus Log Converter . You cannot overwrite the DbFiles property."
---

# IBus.DbFiles

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: DbFiles for Bus

Returns the database files that are associated with a bus in the Bus Log Converter . You cannot overwrite the DbFiles property.

## Signature

```python
return_value = obj.DbFiles
```

## Python example

```python
oMyDbFiles = dd.BusLogToTDM.BusDbConfig.Buses(1).DbFiles
for i in range(1, oMyDbFiles.Count+1):
    dd.MsgBoxDisp(oMyDbFiles(i).File)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_DbFiles_IBus.htm`*

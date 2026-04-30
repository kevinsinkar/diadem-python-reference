---
title: "IDbFileCollection.Count"
description: "Specifies in the Bus Log Converter the number of database files which are assigned to a specific bus. You cannot overwrite the Count property."
---

# IDbFileCollection.Count

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Count for DbFiles

Specifies in the Bus Log Converter the number of database files which are assigned to a specific bus. You cannot overwrite the Count property.

## Signature

```python
obj.Count
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

*Source: `ICANConverter/properties/CANConverter_property_Count_IDbFileCollection.htm`*

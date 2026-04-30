---
title: "ILogFileCollection.Count"
description: "Specifies the number of logfiles to be converted in the Bus Log Converter . You can enter multiple logfiles in GIN-Multilogger files, but only one logfile in al"
---

# ILogFileCollection.Count

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Count for LogFiles

Specifies the number of logfiles to be converted in the Bus Log Converter . You can enter multiple logfiles in GIN-Multilogger files, but only one logfile in all other formats. You cannot overwrite the Count property.

## Signature

```python
obj.Count
```

## Python example

```python
oMyLogFiles = dd.BusLogToTDM.LogSettings.LogFiles
for i in range(1, oMyLogFiles.Count+1):
    dd.MsgBoxDisp(oMyLogFiles(i).File)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Count_ILogFileCollection.htm`*

---
title: "ILogSettings.LogFiles"
description: "Returns all the logfiles that are selected for conversion in the Bus Log Converter . You can only specify several logfiles for GIN-Multilogger files. You cannot"
---

# ILogSettings.LogFiles

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: LogFiles for LogSettings

Returns all the logfiles that are selected for conversion in the Bus Log Converter . You can only specify several logfiles for GIN-Multilogger files. You cannot overwrite the LogFiles property.

## Signature

```python
return_value = obj.LogFiles
```

## Python example

```python
oMyLogfile = dd.BusLogToTDM.LogSettings.LogFiles(1)
dd.MsgBoxDisp(oMyLogfile.File)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_LogFiles_ILogSettings.htm`*

---
title: "ILogFile.DisplayFile"
description: "Specifies the name of a logfile in the Bus Log Converter . The DisplayFile property does not contain the file path. You cannot overwrite the DisplayFile propert"
---

# ILogFile.DisplayFile

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: DisplayFile for LogFile

Specifies the name of a logfile in the Bus Log Converter . The DisplayFile property does not contain the file path. You cannot overwrite the DisplayFile property.

## Signature

```python
obj.DisplayFile
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.LogSettings.LogFiles(1).DisplayFile)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_DisplayFile_ILogFile.htm`*

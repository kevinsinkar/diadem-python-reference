---
title: "ILogFile.XnetTdmsChannels"
description: "Specifies in the Bus Log Converter the names of the channels to be converted in an NI-XNET-TDMS logfile. Only use this property for TDMS logfiles. If you do not"
---

# ILogFile.XnetTdmsChannels

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: XnetTdmsChannels for LogFile

Specifies in the Bus Log Converter the names of the channels to be converted in an NI-XNET-TDMS logfile. Only use this property for TDMS logfiles. If you do not assign channels to this property so that the string is empty, DIAdem converts all channels in the TDMS logfile.

## Signature

```python
return_value = obj.XnetTdmsChannels
```

## Python example

```python
dd.BusLogToTDM.Clear()
dd.BusLogToTDM.LogSettings.FileType = dd.eLogFileTypeTdms
oLogFile = dd.BusLogToTDM.LogSettings.LogFiles.Add("D:\\LogFiles\\Logfile.tdms")
oLogFile.XnetTdmsChannels.Add("XNET_Group1/XNET_Channel1")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_XnetTdmsChannels_ILogFile.htm`*

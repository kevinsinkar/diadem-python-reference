---
title: "IResultSettings.SignalFilter"
description: "Returns the SignalFilter object. The SignalFilter object provides a filter for the Bus Log Converter . If the Active property has the value TRUE , the Bus Log C"
---

# IResultSettings.SignalFilter

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: SignalFilter for ResultSettings

Returns the SignalFilter object. The SignalFilter object provides a filter for the Bus Log Converter . If the Active property has the value TRUE , the Bus Log Converter loads only the signal names (upper or lower case) that are in the filter list.

## Signature

```python
return_value = obj.SignalFilter
```

## Python example

```python
oMySignalFilter = dd.BusLogToTDM.ResultSettings.SignalFilter
oMySignals = oMySignalFilter.Signals
oMySignals.Add("Speed")
oMySignals.Add("Time")
oMySignalFilter.Active = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_SignalFilter_IResultSettings.htm`*

---
title: "ISignalFilter.Signals"
description: "Specifies a string vector containing the names of the signals by which the Bus Log Converter filters. If the Active property has the value TRUE , the Bus Log Co"
---

# ISignalFilter.Signals

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Signals for SignalFilter

Specifies a string vector containing the names of the signals by which the Bus Log Converter filters. If the Active property has the value TRUE , the Bus Log Converter loads only the files (upper or lower case) that are in the filter list.

## Signature

```python
return_value = obj.Signals
```

## Python example

```python
oMySignals = dd.BusLogToTDM.ResultSettings.SignalFilter.Signals
oMySignals.Add("Speed")
oMySignals.Add("Time")
for oMySignal in oMySignals:
    dd.LogfileWrite(oMySignal)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Signals_ISignalFilter.htm`*

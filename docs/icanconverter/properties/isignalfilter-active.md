---
title: "ISignalFilter.Active"
description: "Specifies whether a filter is enabled for the Bus Log Converter . When a filter is enabled, the Bus Log Converter only loads the signals (upper and lowercase) t"
---

# ISignalFilter.Active

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Active for SignalFilter

Specifies whether a filter is enabled for the Bus Log Converter . When a filter is enabled, the Bus Log Converter only loads the signals (upper and lowercase) that are in the filter list.

## Signature

```python
obj.Active
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

*Source: `ICANConverter/properties/CANConverter_property_Active_ISignalFilter.htm`*

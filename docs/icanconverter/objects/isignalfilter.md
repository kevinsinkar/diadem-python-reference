---
title: "ISignalFilter"
description: "The SignalFilter object provides a filter for the Bus Log Converter . If the Active property has the value TRUE , the Bus Log Converter loads only the signal na"
---

# ISignalFilter

!!! abstract "Object &middot; `ICANConverter.chm`"
    Object: SignalFilter

The SignalFilter object provides a filter for the Bus Log Converter . If the Active property has the value TRUE , the Bus Log Converter loads only the signal names (upper or lower case) that are in the filter list.

## Python example

```python
oMySignalFilter = dd.BusLogToTDM.ResultSettings.SignalFilter
oMySignals = oMySignalFilter.Signals
oMySignals.Add("Speed")
oMySignals.Add("Time")
oMySignalFilter.Active = True
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/isignalfilter-active/">Active</a> | <a href="../../properties/isignalfilter-signals/">Signals</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/isignalfilter-load/">Load</a> | <a href="../../methods/isignalfilter-saveas/">SaveAs</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../iresultsettings/">ResultSettings</a>.<a href="../../properties/iresultsettings-signalfilter/">SignalFilter</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_ISignalFilter.htm`*

---
title: "IToStringItemVecUniqueInt.Add"
description: "Adds a text to the string vector containing the names of the signals by which the Bus Log Converter filters."
---

# IToStringItemVecUniqueInt.Add

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Add for UniqueStringVector

Adds a text to the string vector containing the names of the signals by which the Bus Log Converter filters.

## Signature

```python
obj.Add(Value)
```

## Python example

```python
oMySignals = dd.BusLogToTDM.ResultSettings.SignalFilter.Signals
oMySignals.Add("Speed")
oMySignals.Add("Time")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Add_IToStringItemVecUniqueInt.htm`*

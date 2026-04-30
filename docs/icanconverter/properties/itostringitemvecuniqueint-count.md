---
title: "IToStringItemVecUniqueInt.Count"
description: "Returns the number of texts in the string vector containing the names of the signals by which the Bus Log Converter filters."
---

# IToStringItemVecUniqueInt.Count

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Count for UniqueStringVector

Returns the number of texts in the string vector containing the names of the signals by which the Bus Log Converter filters.

## Signature

```python
obj.Count
```

## Python example

```python
oMySignals = dd.BusLogToTDM.ResultSettings.SignalFilter.Signals
oMySignals.Add("Speed")
oMySignals.Add("Time")
for i in range(1, oMySignals.Count+1):
    dd.LogfileWrite(oMySignals(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Count_IToStringItemVecUniqueInt.htm`*

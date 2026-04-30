---
title: "UniqueStringVector"
description: "Collection of all filter texts in the Bus Log Converter ."
---

# UniqueStringVector

!!! abstract "Collection &middot; `ICANConverter.chm`"
    Collection: UniqueStringVector

Collection of all filter texts in the Bus Log Converter .

## Python example

```python
oMySignals = dd.BusLogToTDM.ResultSettings.SignalFilter.Signals
oMySignals.Add("Speed")
oMySignals.Add("Time")
for oMySignal in oMySignals:
    dd.LogfileWrite(oMySignal)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/itostringitemvecuniqueint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/itostringitemvecuniqueint-add/">Add</a> | <a href="../../methods/itostringitemvecuniqueint-item/">Item</a> | <a href="../../methods/itostringitemvecuniqueint-remove/">Remove</a> | <a href="../../methods/itostringitemvecuniqueint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/isignalfilter/">SignalFilter</a>.<a href="../../properties/isignalfilter-signals/">Signals</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_IToStringItemVecUniqueInt.htm`*

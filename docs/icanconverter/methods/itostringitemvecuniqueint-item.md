---
title: "IToStringItemVecUniqueInt.Item"
description: "Specifies in the Bus Log Converter filter text associated with a specific index."
---

# IToStringItemVecUniqueInt.Item

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Item for UniqueStringVector

Specifies in the Bus Log Converter filter text associated with a specific index.

## Signature

```python
sItem = Object.Item(Index)
```

## Notes

<div markdown="1">
<table class="Borderless"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMySignals = dd.BusLogToTDM.ResultSettings.SignalFilter.Signals
for i in range(1, oMySignals.Count+1):
    dd.LogfileWrite(oMySignals.Items(i))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Item_IToStringItemVecUniqueInt.htm`*

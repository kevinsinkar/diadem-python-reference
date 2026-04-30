---
title: "IBusFilterBusCollection.Item"
description: "Returns the bus that is associated with a specific index or name from a filtered bus collection, in the Bus Log Converter ."
---

# IBusFilterBusCollection.Item

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Item for UsedBuses

Returns the bus that is associated with a specific index or name from a filtered bus collection, in the Bus Log Converter .

## Signature

```python
return_value = obj.Item(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You can always omit the <span class="Monospace">Item</span> method because it is the standard element of the collection.</td></tr></table>
</div>

## Python example

```python
oMyBus =dd.BusLogToTDM.ResultSettings.BusFilter.UsedBuses.Item(1)

oMyBus =dd.BusLogToTDM.ResultSettings.BusFilter.UsedBuses(1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Item_IBusFilterBusCollection.htm`*

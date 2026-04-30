---
title: "IBus"
description: "The Bus object makes a specific bus available in the Bus Log Converter . You can use the Bus object to access the name and the number of the bus and to access t"
---

# IBus

!!! abstract "Object &middot; `ICANConverter.chm`"
    Object: Bus

The Bus object makes a specific bus available in the Bus Log Converter . You can use the Bus object to access the name and the number of the bus and to access the database files that are assigned to the bus.

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses(1).Name)
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ibus-dbfiles/">DbFiles</a> | <a href="../../properties/ibus-name/">Name</a> | <a href="../../properties/ibus-number/">Number</a> | <a href="../../properties/ibus-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/buses/">Buses</a>.<a href="../../methods/ibuscollection-add/">Add</a> | <a href="../../collections/buses/">Buses</a>.<a href="../../methods/ibuscollection-addbytype/">AddByType</a> | <a href="../../collections/buses/">Buses</a>.<a href="../../methods/ibuscollection-item/">Item</a> | <a href="../../collections/usedbuses/">UsedBuses</a>.<a href="../../methods/ibusfilterbuscollection-add/">Add</a> | <a href="../../collections/usedbuses/">UsedBuses</a>.<a href="../../methods/ibusfilterbuscollection-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/objects/CANConverter_Objects_IBus.htm`*

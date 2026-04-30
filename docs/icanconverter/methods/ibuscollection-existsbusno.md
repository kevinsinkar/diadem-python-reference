---
title: "IBusCollection.ExistsBusNo"
description: "Use the ExistsBusNoByType method instead of the ExistsBusNo method to check whether a bus with a certain number and a specific type already exists in the Buses "
---

# IBusCollection.ExistsBusNo

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: ExistsBusNo for Buses

Use the ExistsBusNoByType method instead of the ExistsBusNo method to check whether a bus with a certain number and a specific type already exists in the Buses collection. Checks in the Bus Log Converter whether a CAN bus with a specific number already exists.

## Signature

```python
bExistsBusNo = Object.ExistsBusNo(BusNumber)
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses.ExistsBusNo(2))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_ExistsBusNo_IBusCollection.htm`*

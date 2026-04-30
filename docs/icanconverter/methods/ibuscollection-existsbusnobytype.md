---
title: "IBusCollection.ExistsBusNoByType"
description: "Checks in the Bus Log Converter whether a bus with a certain number and a specific type already exists in the Buses collection."
---

# IBusCollection.ExistsBusNoByType

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: ExistsBusNoByType for Buses

Checks in the Bus Log Converter whether a bus with a certain number and a specific type already exists in the Buses collection.

## Signature

```python
bExistsBusNoByType = Object.ExistsBusNoByType(BusNumber, BusType)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eBusTypeUndefined` | 0 | Not defined |
| `eBusTypeCAN` | 1 | CAN |
| `eBusTypeLIN` | 2 | LIN |
| `eBusTypeFLEXRAY` | 3 | Flexray |

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses.ExistsBusNoByType(2,dd.eBusTypeCAN))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_ExistsBusNoByType_IBusCollection.htm`*

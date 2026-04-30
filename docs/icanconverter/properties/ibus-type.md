---
title: "IBus.Type"
description: "Specifies the type of a bus in the Bus Log Converter . You cannot overwrite the Type property."
---

# IBus.Type

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Type for Bus

Specifies the type of a bus in the Bus Log Converter . You cannot overwrite the Type property.

## Signature

```python
obj.Type
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
dd.MsgBoxDisp(dd.BusLogToTDM.BusDbConfig.Buses("CAN2").Type)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Type_IBus.htm`*

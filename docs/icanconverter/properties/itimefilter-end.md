---
title: "ITimeFilter.End"
description: "Specifies the end value for the time filter in seconds in the Bus Log Converter . The time filter specifies the section of the logfile which you can convert int"
---

# ITimeFilter.End

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: End for TimeFilter

Specifies the end value for the time filter in seconds in the Bus Log Converter . The time filter specifies the section of the logfile which you can convert into the TDM file. Use the Begin property to specify the start value of the time filter.

## Signature

```python
obj.End
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.ResultSettings.TimeFilter.End)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_End_ITimeFilter.htm`*

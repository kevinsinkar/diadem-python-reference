---
title: "ITimeFilter.Begin"
description: "Specifies the start value for the time filter in seconds in the Bus Log Converter . The time filter specifies the section of the logfile which you can convert i"
---

# ITimeFilter.Begin

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Begin for TimeFilter

Specifies the start value for the time filter in seconds in the Bus Log Converter . The time filter specifies the section of the logfile which you can convert into the TDM file. Use the End property to specify the end value of the time filter.

## Signature

```python
obj.Begin
```

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.ResultSettings.TimeFilter.Begin)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Begin_ITimeFilter.htm`*

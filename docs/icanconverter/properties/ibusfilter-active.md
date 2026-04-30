---
title: "IBusFilter.Active"
description: "Specifies whether the filter, which converts only specific buses in the logfiles and not all the buses that are referenced in the logfiles, is active in the Bus"
---

# IBusFilter.Active

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: Active for BusFilter

Specifies whether the filter, which converts only specific buses in the logfiles and not all the buses that are referenced in the logfiles, is active in the Bus Log Converter .

## Signature

```python
obj.Active
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>Even if a bus filter is active, you must still configure all the buses that are configured in the logfile.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.ResultSettings.BusFilter.Active)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_Active_IBusFilter.htm`*

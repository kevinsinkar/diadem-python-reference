---
title: "ICANConverter.FileName"
description: "Returns in the Bus Log Converter the filename of the file that contains the Bus Log Converter settings. You cannot overwrite the FileName property."
---

# ICANConverter.FileName

!!! abstract "Property &middot; `ICANConverter.chm`"
    Property: FileName for BusLogToTDM

Returns in the Bus Log Converter the filename of the file that contains the Bus Log Converter settings. You cannot overwrite the FileName property.

## Signature

```python
obj.FileName
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>You use the methods <a href="../../methods/icanconverter-saveas/">SaveAs</a>, <a href="../../methods/icanconverter-clear/">Clear</a>, and <a href="../../methods/icanconverter-load/">Load</a> to assign a value to the <span class="Monospace">FileName</span> property.</td></tr></table>
</div>

## Python example

```python
dd.MsgBoxDisp(dd.BusLogToTDM.FileName)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/properties/CANConverter_property_FileName_ICANConverter.htm`*

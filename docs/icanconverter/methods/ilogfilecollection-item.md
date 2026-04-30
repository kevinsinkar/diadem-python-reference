---
title: "ILogFileCollection.Item"
description: "Returns the logfile that is associated with a specific index or name, in the Bus Log Converter ."
---

# ILogFileCollection.Item

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Item for LogFiles

Returns the logfile that is associated with a specific index or name, in the Bus Log Converter .

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
dd.MsgBoxDisp(dd.BusLogToTDM.LogSettings.LogFiles.Item(1).File)

dd.MsgBoxDisp(dd.BusLogToTDM.LogSettings.LogFiles(1).File)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Item_ILogFileCollection.htm`*

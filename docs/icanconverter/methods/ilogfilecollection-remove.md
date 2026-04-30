---
title: "ILogFileCollection.Remove"
description: "Deletes an element from the LogFiles collection , in the Bus Log Converter ."
---

# ILogFileCollection.Remove

!!! abstract "Method &middot; `ICANConverter.chm`"
    Method: Remove for LogFiles

Deletes an element from the LogFiles collection , in the Bus Log Converter .

## Signature

```python
obj.Remove(NameOrIndex)
```

## Notes

<div markdown="1">
<table class="Borderless" id="table1"><tr><td class="Icon"><img src="../image/note.gif"/></td><td><strong>Note  </strong>It is recommended to specify several logfiles only when you convert GIN files.</td></tr></table>
</div>

## Python example

```python
dd.BusLogToTDM.LogSettings.LogFiles.Remove(1)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Converting a Bus Logfile into the TDM Format</a></p>
</div>
</div>

---

*Source: `ICANConverter/methods/CANConverter_method_Remove_ILogFileCollection.htm`*

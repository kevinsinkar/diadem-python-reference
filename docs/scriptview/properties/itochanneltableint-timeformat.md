---
title: "IToChannelTableInt.TimeFormat"
description: "Specifies the time format for all the columns of a channel table in DIAdem VIEW."
---

# IToChannelTableInt.TimeFormat

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: TimeFormat for ChannelTable

Specifies the time format for all the columns of a channel table in DIAdem VIEW.

## Signature

```python
obj.TimeFormat
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
dd.View.Sheets(1).Areas(1).DisplayObj.TimeFormat = "#mm/dd/yy hh:nn:ss"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_TimeFormat_IToChannelTableInt.htm`*

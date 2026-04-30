---
title: "IToChannelTableInt.Area"
description: "Returns the area in DIAdem VIEW that contains a channel table."
---

# IToChannelTableInt.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for ChannelTable

Returns the area in DIAdem VIEW that contains a channel table.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "ChannelTable"
oMyDisplayObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyDisplayObj.Columns.Add("[1]/[3]")
dd.MsgBoxDisp("Name " + oMyDisplayObj.Area.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_IToChannelTableInt.htm`*

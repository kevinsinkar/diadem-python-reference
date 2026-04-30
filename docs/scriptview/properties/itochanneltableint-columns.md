---
title: "IToChannelTableInt.Columns"
description: "Returns a collection of the columns in a channel table in DIAdem VIEW."
---

# IToChannelTableInt.Columns

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Columns for ChannelTable

Returns a collection of the columns in a channel table in DIAdem VIEW.

## Signature

```python
return_value = obj.Columns
```

## Python example

```python
for oChannel in dd.View.ActiveSheet.ActiveArea.DisplayObj.Columns:
    oChannel.Format = "d.dd"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Columns_IToChannelTableInt.htm`*

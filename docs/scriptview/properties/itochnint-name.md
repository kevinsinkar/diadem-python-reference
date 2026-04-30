---
title: "IToChnInt.Name"
description: "Specifies the name of a column of a channel table in DIAdem VIEW."
---

# IToChnInt.Name

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Name for Column

Specifies the name of a column of a channel table in DIAdem VIEW.

## Signature

```python
obj.Name
```

## Python example

```python
oMyTab = dd.View.ActiveSheet.ActiveArea.DisplayObj
for i in range(1, oMyTab.Columns.Count+1):
    dd.MsgBoxDisp("Column name: " + oMyTab.Columns(i).Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p><h2>Procedures</h2><p><a href="#" data-unresolved="1">Block Operations in Channel Tables</a> | <a href="#" data-unresolved="1">Changing a Table Display</a> | <a href="#" data-unresolved="1">Cutting, Copying, and Pasting Data Blocks into Channel Tables</a> | <a href="#" data-unresolved="1">Deleting Channel Table Columns</a> | <a href="#" data-unresolved="1">Displaying All Channels in One Channel Table</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Name_IToChnInt.htm`*

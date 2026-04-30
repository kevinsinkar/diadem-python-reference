---
title: "IToAttrEnumInt.Add"
description: "Adds an object to the LegendItems collection and returns a LegendItems object, in the script interface of DIAdem VIEW."
---

# IToAttrEnumInt.Add

!!! abstract "Method &middot; `Scriptview.chm`"
    Method: Add for LegendItems

Adds an object to the LegendItems collection and returns a LegendItems object, in the script interface of DIAdem VIEW.

## Signature

```python
return_value = obj.Add(AttrName)
```

## Python example

```python
dd.View.Sheets.RemoveAll()
oMySheet = dd.View.Sheets.Add("NewSheet")
oOldArea = oMySheet.ActiveArea
oOldArea.DisplayObjType = "CurveChart2D"
oOldArea.DisplayObj.Curves2D.Add("[1]/[1]","[1]/[3]")
oOldArea.DisplayObj.LegendItems.Add("Name")
oNewArea = oMySheet.ActiveArea.SplitTop("NewArea",0.5)
oNewArea.DisplayObjType = "ChannelTable"
oNewArea.DisplayObj.Columns.Add(3)
oNewArea.DisplayObj.HeaderItems.Add("Name")
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/methods/VIEW_method_Add_IToAttrEnumInt.htm`*

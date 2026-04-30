---
title: "ITo2DChartInt.Area"
description: "Returns the area in DIAdem VIEW that contains the 2D axis system."
---

# ITo2DChartInt.Area

!!! abstract "Property &middot; `Scriptview.chm`"
    Property: Area for CurveChart2D

Returns the area in DIAdem VIEW that contains the 2D axis system.

## Signature

```python
return_value = obj.Area
```

## Python example

```python
dd.View.Sheets(1).Areas(1).DisplayObjType = "CurveChart2D"
oMyDisplayObj = dd.View.Sheets(1).Areas(1).DisplayObj
oMyDisplayObj.Curves2D.Add("[2]/[1]","[2]/[2]")
dd.MsgBoxDisp("Name " + oMyDisplayObj.Area.Name)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p class="body"><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `Scriptview/properties/VIEW_property_Area_ITo2DChartInt.htm`*

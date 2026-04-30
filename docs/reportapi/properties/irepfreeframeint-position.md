---
title: "IRepFreeFrameInt.Position"
description: "Specifies the position of a rectangle in a DIAdem REPORT worksheet."
---

# IRepFreeFrameInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for Frame

Specifies the position of a rectangle in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyBackgroundColor = oMyFrame.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed)
oMyPosition = oMyFrame.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 50
oMyPosition.Y2 = 80
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepFreeFrameInt.htm`*

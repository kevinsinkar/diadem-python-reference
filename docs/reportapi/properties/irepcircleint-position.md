---
title: "IRepCircleInt.Position"
description: "Specifies the position of a circle in a DIAdem REPORT worksheet."
---

# IRepCircleInt.Position

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Position for Circle

Specifies the position of a circle in a DIAdem REPORT worksheet.

## Signature

```python
return_value = obj.Position
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.ForceCircle = True
oMyBackgroundColor = oMyCircle.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyPosition = oMyCircle.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 50
oMyPosition.Y2 = 80
oMyBorderLine = oMyCircle.BorderLine
oMyBorderLine.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMyBorderLine.LineType = dd.eLineTypeDotted
oMyBorderLine.Width = dd.eLineWidth0140
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Position_IRepCircleInt.htm`*

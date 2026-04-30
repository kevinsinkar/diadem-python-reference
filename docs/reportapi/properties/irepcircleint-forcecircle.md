---
title: "IRepCircleInt.ForceCircle"
description: "Specifies whether DIAdem REPORT displays a circle or an ellipse."
---

# IRepCircleInt.ForceCircle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ForceCircle for Circle

Specifies whether DIAdem REPORT displays a circle or an ellipse.

## Signature

```python
obj.ForceCircle
```

## Python example

```python
dd.Report.NewLayout()
oMyCircle = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectCircle,"MyCircle")
oMyCircle.ForceCircle = True
oMyBackgroundColor = oMyCircle.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed)
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

*Source: `ReportApi/properties/Report_property_ForceCircle_IRepCircleInt.htm`*

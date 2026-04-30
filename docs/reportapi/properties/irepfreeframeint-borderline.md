---
title: "IRepFreeFrameInt.BorderLine"
description: "Specifies the display of the frame line of a rectangle in DIAdem REPORT."
---

# IRepFreeFrameInt.BorderLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BorderLine for Frame

Specifies the display of the frame line of a rectangle in DIAdem REPORT.

## Signature

```python
return_value = obj.BorderLine
```

## Python example

```python
dd.Report.NewLayout()
oMyFrame = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectFrame,"MyFrame")
oMyBackgroundColor = oMyFrame.BackgroundColor
oMyBackgroundColor.SetPredefinedColor(dd.eColorIndexRed )
oMyPosition = oMyFrame.Position.ByCoordinate
oMyPosition.X1 = 10
oMyPosition.X2 = 40
oMyPosition.Y1 = 50
oMyPosition.Y2 = 80
oMyBorderLine = oMyFrame.BorderLine
oMyBorderLine.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMyBorderLine.LineType = dd.eLineTypeDotted
oMyBorderLine.Width = dd.eLineWidth0140
oMyShadow = oMyFrame.Shadow
oMyShadow.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShadow.Direction = dd.eShadowDirectionLeftBottom
oMyShadow.OffsetX = 1
oMyShadow.OffsetY = 2
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BorderLine_IRepFreeFrameInt.htm`*

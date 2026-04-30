---
title: "IRepShadowInt.OffsetY"
description: "Specifies the vertical displacement of the shadow for rectangles in DIAdem REPORT."
---

# IRepShadowInt.OffsetY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: OffsetY for Shadow

Specifies the vertical displacement of the shadow for rectangles in DIAdem REPORT.

## Signature

```python
obj.OffsetY
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
oMyShadow = oMyFrame.Shadow
oMyShadow.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShadow.Direction = dd.eShadowDirectionLeftBottom
oMyShadow.OffsetX = 1
oMyShadow.OffsetY = 2
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_OffsetY_IRepShadowInt.htm`*

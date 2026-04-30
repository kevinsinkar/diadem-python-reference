---
title: "IRepShadowInt.Color"
description: "Specifies the shadow color of a rectangle or a circle in DIAdem REPORT."
---

# IRepShadowInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for Shadow

Specifies the shadow color of a rectangle or a circle in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
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

*Source: `ReportApi/properties/Report_property_Color_IRepShadowInt.htm`*

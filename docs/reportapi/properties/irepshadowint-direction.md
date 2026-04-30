---
title: "IRepShadowInt.Direction"
description: "Specifies whether and how DIAdem REPORT displays the shadow of a rectangle."
---

# IRepShadowInt.Direction

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Direction for Shadow

Specifies whether and how DIAdem REPORT displays the shadow of a rectangle.

## Signature

```python
obj.Direction
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eShadowDirectionNone` | 0 | No shadow |
| `eShadowDirectionRightBottom` | 1 | Bottom right |
| `eShadowDirectionRightTop` | 2 | Top right |
| `eShadowDirectionLeftBottom` | 3 | Bottom left |
| `eShadowDirectionLeftTop` | 4 | Top left |

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

*Source: `ReportApi/properties/Report_property_Direction_IRepShadowInt.htm`*

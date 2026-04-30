---
title: "IRepLegendPositionAnchorInt.SystemRelatedY"
description: "Specifies the distance between the reference point of the legend of an axis system and the lower edge of the axis system as a percentage of the height of the ax"
---

# IRepLegendPositionAnchorInt.SystemRelatedY

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SystemRelatedY for LegendPositionAnchor

Specifies the distance between the reference point of the legend of an axis system and the lower edge of the axis system as a percentage of the height of the axis system. You must assign the value eLegendAnchorTypeSystemRelated to the Type in order to use the SystemRelatedY property.

## Signature

```python
obj.SystemRelatedY
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve1")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.Type = dd.eLegendAnchorTypeSystemRelated
oMyAnchor.SystemRelatedX = -10
oMyAnchor.SystemRelatedY = -10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SystemRelatedY_IRepLegendPositionAnchorInt.htm`*

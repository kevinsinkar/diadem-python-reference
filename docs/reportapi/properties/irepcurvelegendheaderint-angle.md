---
title: "IRepCurveLegendHeaderInt.Angle"
description: "Specifies the angle in degrees at which DIAdem REPORT displays the title of a curve legend of a 2D axis system."
---

# IRepCurveLegendHeaderInt.Angle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Angle for CurveLegendHeader

Specifies the angle in degrees at which DIAdem REPORT displays the title of a curve legend of a 2D axis system.

## Signature

```python
obj.Angle
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngle0` | 0 |  |
| `eAngle090` | 1 | 90 |
| `eAngle180` | 2 | 180 |
| `eAngle270` | 3 | 270 |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyAnchor = oMyLegend.Position.Anchor
oMyAnchor.PageRelatedX = 70
oMyAnchor.PageRelatedY = 15
oMyLegend.Columns(1).Title = "Legend Title"
oMyLegendHeader = oMyLegend.Header
oMyLegendHeader.ShowGrid = True
oMyLegendHeader.PortionHeaderField = 10
oMyLegendHeader.UseAutoFontSize = False
oMyLegendHeader.Font.Size = 2
oMyLegendHeader.Angle = dd.eAngle090
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Angle_IRepCurveLegendHeaderInt.htm`*

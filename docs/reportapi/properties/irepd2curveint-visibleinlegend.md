---
title: "IRepD2CurveInt.VisibleInLegend"
description: "Specifies whether DIAdem REPORT displays the legend entry of a curve in a 2D axis system."
---

# IRepD2CurveInt.VisibleInLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: VisibleInLegend for 2DCurve

Specifies whether DIAdem REPORT displays the legend entry of a curve in a 2D axis system.

## Signature

```python
obj.VisibleInLegend
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMy2DAxisSystem.CurveLegend.Visible = True
oMy2DCurve.VisibleInLegend = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_VisibleInLegend_IRepD2CurveInt.htm`*

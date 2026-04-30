---
title: "IRepCurveLegendInt.Frame"
description: "Specifies the properties of the curve legend frame in an axis system in DIAdem REPORT."
---

# IRepCurveLegendInt.Frame

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Frame for CurveLegend

Specifies the properties of the curve legend frame in an axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Frame
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.X2 = 80
oMyPosition.Y1 = 20
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyCurveLegend = oMy2DAxisSystem.CurveLegend
oMyCurveLegend.Visible = True
oMyFrame = oMyCurveLegend.Frame
oMyFrame.Visible = True
oMyFrame.Color.ColorIndex = dd.eColorIndexDarkGreen
oMyFrame.LineType = dd.eLineTypeSolid
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Frame_IRepCurveLegendInt.htm`*

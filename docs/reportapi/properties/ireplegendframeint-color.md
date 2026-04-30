---
title: "IRepLegendFrameInt.Color"
description: "Specifies the frame color of a curve legend and a color legend in DIAdem REPORT."
---

# IRepLegendFrameInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for LegendFrame

Specifies the frame color of a curve legend and a color legend in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyLegendFrame = oMyLegend.Frame
oMyLegendFrame.Visible = True
oMyLegendFrame.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyLegendFrame.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepLegendFrameInt.htm`*

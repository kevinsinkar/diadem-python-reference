---
title: "IRepLegendFrameInt"
description: "The LegendFrame object provides the frame properties of a curve legend and a color legend in DIAdem REPORT."
---

# IRepLegendFrameInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LegendFrame

The LegendFrame object provides the frame properties of a curve legend and a color legend in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplegendframeint-color/">Color</a> | <a href="../../properties/ireplegendframeint-linetype/">LineType</a> | <a href="../../properties/ireplegendframeint-visible/">Visible</a> | <a href="../../properties/ireplegendframeint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcolorlegendint/">ColorLegend</a>.<a href="../../properties/irepcolorlegendint-frame/">Frame</a> | <a href="../irepcurvelegendint/">CurveLegend</a>.<a href="../../properties/irepcurvelegendint-frame/">Frame</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLegendFrameInt.htm`*

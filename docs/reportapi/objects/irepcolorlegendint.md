---
title: "IRepColorLegendInt"
description: "The ColorLegend object provides a color legend in DIAdem REPORT."
---

# IRepColorLegendInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ColorLegend

The ColorLegend object provides a color legend in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 60
oMyPos.Y1 = 20
oMyPos.Y2 = 60
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Settings.Line.Color.ColorIndex = dd.eColorIndexPalette
oMyColorLegend = oMy2DAxisSystem.ColorLegend
oMyColorLegend.Visible = True
oMyNumbers = oMyColorLegend.Settings.Numbers
oMyNumbers.Format = "d.ddde"
oMyNumbers.Mode = dd.eColorLegendScaleSingleValue
oMyNumbers.ValueMode = dd.eColorLegendScaleValueModeCenter
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcolorlegendint-frame/">Frame</a> | <a href="../../properties/irepcolorlegendint-header/">Header</a> | <a href="../../properties/irepcolorlegendint-position/">Position</a> | <a href="../../properties/irepcolorlegendint-settings/">Settings</a> | <a href="../../properties/irepcolorlegendint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-colorlegend/">ColorLegend</a> | <a href="../irepd3axisint/">3DAxisSystem</a>.<a href="../../properties/irepd3axisint-colorlegend/">ColorLegend</a> | <a href="../irepd3shapeobjcharacteristicdiagramsettingsint/">3DCharacteristicDiagramSettings</a>.<a href="../../properties/irepd3shapeobjcharacteristicdiagramsettingsint-colorlegend/">ColorLegend</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepColorLegendInt.htm`*

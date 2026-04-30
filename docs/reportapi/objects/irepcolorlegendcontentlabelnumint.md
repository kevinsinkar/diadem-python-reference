---
title: "IRepColorLegendContentLabelNumInt"
description: "The ColorLegendNumbers object provides the label numbers of a color legend in DIAdem REPORT."
---

# IRepColorLegendContentLabelNumInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ColorLegendNumbers

The ColorLegendNumbers object provides the label numbers of a color legend in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
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
<p><a href="../../properties/irepcolorlegendcontentlabelnumint-format/">Format</a> | <a href="../../properties/irepcolorlegendcontentlabelnumint-interval/">Interval</a> | <a href="../../properties/irepcolorlegendcontentlabelnumint-mode/">Mode</a> | <a href="../../properties/irepcolorlegendcontentlabelnumint-onlyfirstandlast/">OnlyFirstAndLast</a> | <a href="../../properties/irepcolorlegendcontentlabelnumint-usepalettecolor/">UsePaletteColor</a> | <a href="../../properties/irepcolorlegendcontentlabelnumint-valuemode/">ValueMode</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcolorlegendsettingsint/">ColorLegendSettings</a>.<a href="../../properties/irepcolorlegendsettingsint-numbers/">Numbers</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepColorLegendContentLabelNumInt.htm`*

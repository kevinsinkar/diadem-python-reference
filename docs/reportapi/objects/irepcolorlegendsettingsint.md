---
title: "IRepColorLegendSettingsInt"
description: "The ColorLegendSettings object provides the properties of a color legend in DIAdem REPORT."
---

# IRepColorLegendSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ColorLegendSettings

The ColorLegendSettings object provides the properties of a color legend in DIAdem REPORT.

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
<p><a href="../../properties/irepcolorlegendsettingsint-alignment/">Alignment</a> | <a href="../../properties/irepcolorlegendsettingsint-angle/">Angle</a> | <a href="../../properties/irepcolorlegendsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepcolorlegendsettingsint-expansiondirection/">ExpansionDirection</a> | <a href="../../properties/irepcolorlegendsettingsint-font/">Font</a> | <a href="../../properties/irepcolorlegendsettingsint-numbers/">Numbers</a> | <a href="../../properties/irepcolorlegendsettingsint-orientation/">Orientation</a> | <a href="../../properties/irepcolorlegendsettingsint-portionsymbolfield/">PortionSymbolField</a> | <a href="../../properties/irepcolorlegendsettingsint-showsymbolframe/">ShowSymbolFrame</a> | <a href="../../properties/irepcolorlegendsettingsint-symbolspace/">SymbolSpace</a> | <a href="../../properties/irepcolorlegendsettingsint-symboltype/">SymbolType</a> | <a href="../../properties/irepcolorlegendsettingsint-useautofontsize/">UseAutoFontSize</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcolorlegendint/">ColorLegend</a>.<a href="../../properties/irepcolorlegendint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepColorLegendSettingsInt.htm`*

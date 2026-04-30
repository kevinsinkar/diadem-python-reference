---
title: "IRepCurveLegendSettingsInt"
description: "The CurveLegendSettings object provides the curve legend properties in DIAdem REPORT."
---

# IRepCurveLegendSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CurveLegendSettings

The CurveLegendSettings object provides the curve legend properties in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyLegend = oMy2DAxisSystem.CurveLegend
oMyLegend.Visible = True
oMyLegend.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexGrey)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcurvelegendsettingsint-alignment/">Alignment</a> | <a href="../../properties/irepcurvelegendsettingsint-angle/">Angle</a> | <a href="../../properties/irepcurvelegendsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/irepcurvelegendsettingsint-expansiondirection/">ExpansionDirection</a> | <a href="../../properties/irepcurvelegendsettingsint-font/">Font</a> | <a href="../../properties/irepcurvelegendsettingsint-orientation/">Orientation</a> | <a href="../../properties/irepcurvelegendsettingsint-portionsymbolfield/">PortionSymbolField</a> | <a href="../../properties/irepcurvelegendsettingsint-showgridlines/">ShowGridLines</a> | <a href="../../properties/irepcurvelegendsettingsint-showonlyfirstcurve/">ShowOnlyFirstCurve</a> | <a href="../../properties/irepcurvelegendsettingsint-showsymbolframe/">ShowSymbolFrame</a> | <a href="../../properties/irepcurvelegendsettingsint-useautofontsize/">UseAutoFontSize</a> | <a href="../../properties/irepcurvelegendsettingsint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepcurvelegendsettingsint-useextendedsettings/">UseExtendedSettings</a> | <a href="../../properties/irepcurvelegendsettingsint-usetextclipping/">UseTextClipping</a> | <a href="../../properties/irepcurvelegendsettingsint-usewordwrap/">UseWordWrap</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepcurvelegendint/">CurveLegend</a>.<a href="../../properties/irepcurvelegendint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCurveLegendSettingsInt.htm`*

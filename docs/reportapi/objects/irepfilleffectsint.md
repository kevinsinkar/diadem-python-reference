---
title: "IRepFillEffectsInt"
description: "The FillEffects object provides the properties of the curve filling in a 2D axis system in DIAdem REPORT."
---

# IRepFillEffectsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: FillEffects

The FillEffects object provides the properties of the curve filling in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeFilledArea, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Line.Width = dd.eLineWidth0100
oMyFillEffect = oMySettings.FillEffects
oMyFillEffect.Color.SetFillingColor(255,0,dd.eColorGradientDiagonalRight,dd.eColorGradientModeFromInside)
oMyFillEffect.Pattern = dd.eFillPatternLeftDiagonal
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepfilleffectsint-color/">Color</a> | <a href="../../properties/irepfilleffectsint-gradientmode/">GradientMode</a> | <a href="../../properties/irepfilleffectsint-pattern/">Pattern</a> | <a href="../../properties/irepfilleffectsint-patterntype/">PatternType</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjfilledareasettingsint/">2DFilledAreaSettings</a>.<a href="../../properties/irepd2shapeobjfilledareasettingsint-filleffects/">FillEffects</a> | <a href="../irepd2shapeobjlineandpointssettingsint/">2DLineAndPointsSettings</a>.<a href="../../properties/irepd2shapeobjlineandpointssettingsint-filleffects/">FillEffects</a> | <a href="../irepd2shapeobjlinesettingsint/">2DLineSettings</a>.<a href="../../properties/irepd2shapeobjlinesettingsint-filleffects/">FillEffects</a> | <a href="../irepd2shapeobjoutlbarshorizontalsettingsint/">2DOutlineBarsHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjoutlbarshorizontalsettingsint-filleffects/">FillEffects</a> | <a href="../irepd2shapeobjoutlbarssettingsint/">2DOutlineBarsSettings</a>.<a href="../../properties/irepd2shapeobjoutlbarssettingsint-filleffects/">FillEffects</a> | <a href="../irepd2shapeobjspecialcombinationsettingsint/">2DSpecialCombinationSettings</a>.<a href="../../properties/irepd2shapeobjspecialcombinationsettingsint-filleffects/">FillEffects</a> | <a href="../irepspidershapeobjlineandpointssettingsint/">SpiderLineAndPointsSettings</a>.<a href="../../properties/irepspidershapeobjlineandpointssettingsint-filleffects/">FillEffects</a> | <a href="../irepspidershapeobjlinesettingsint/">SpiderLineSettings</a>.<a href="../../properties/irepspidershapeobjlinesettingsint-filleffects/">FillEffects</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepFillEffectsInt.htm`*

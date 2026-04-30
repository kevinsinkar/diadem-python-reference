---
title: "IRepD2ShapeObjOutlBarsSettingsInt"
description: "The 2DOutlineBarsHorizontalSettings object provides the curve parameter properties of a 2D axis system in the Outline display mode in DIAdem REPORT."
---

# IRepD2ShapeObjOutlBarsSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DOutlineBarsSettings

The 2DOutlineBarsHorizontalSettings object provides the curve parameter properties of a 2D axis system in the Outline display mode in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeOutlineBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySettings = oMyShape.Settings
oMySettings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.FillEffects.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjoutlbarssettingsint-filleffects/">FillEffects</a> | <a href="../../properties/irepd2shapeobjoutlbarssettingsint-line/">Line</a> | <a href="../../properties/irepd2shapeobjoutlbarssettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjoutlbarssettingsint-type/">Type</a> | <a href="../../properties/irepd2shapeobjoutlbarssettingsint-usecurveexpansion/">UseCurveExpansion</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjoutlinebarsint/">2DOutlineBars</a>.<a href="../../properties/irepd2shapeobjoutlinebarsint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjOutlBarsSettingsInt.htm`*

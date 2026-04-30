---
title: "IRepD2ShapeObjBarsSettingsInt"
description: "The 2DBarsSettings object provides the curve parameter properties of a 2D axis system in the Bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBarsSettings

The 2DBarsSettings object provides the curve parameter properties of a 2D axis system in the Bars display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = ""
oMyShape.YChannel.Reference = "[4]/[1]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.Filling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjbarssettingsint-borderline/">BorderLine</a> | <a href="../../properties/irepd2shapeobjbarssettingsint-displaymode/">DisplayMode</a> | <a href="../../properties/irepd2shapeobjbarssettingsint-filling/">Filling</a> | <a href="../../properties/irepd2shapeobjbarssettingsint-offset/">Offset</a> | <a href="../../properties/irepd2shapeobjbarssettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjbarssettingsint-usecurveexpansion/">UseCurveExpansion</a> | <a href="../../properties/irepd2shapeobjbarssettingsint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjbarsint/">2DBars</a>.<a href="../../properties/irepd2shapeobjbarsint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBarsSettingsInt.htm`*

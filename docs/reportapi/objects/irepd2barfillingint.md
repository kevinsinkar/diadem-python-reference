---
title: "IRepD2BarFillingInt"
description: "The 2DBarFilling object provides the properties of a bar display in a 2D axis system in DIAdem REPORT."
---

# IRepD2BarFillingInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DBarFilling

The 2DBarFilling object provides the properties of a bar display in a 2D axis system in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFilling = oMySettings.Filling
oMyFilling.UseSameColorAsBorder = False
oMyFilling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyFilling.Pattern = dd.eFillPatternCrossDiagonal
oMyFilling.Density = 30
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2barfillingint-color/">Color</a> | <a href="../../properties/irepd2barfillingint-density/">Density</a> | <a href="../../properties/irepd2barfillingint-linewidth/">LineWidth</a> | <a href="../../properties/irepd2barfillingint-pattern/">Pattern</a> | <a href="../../properties/irepd2barfillingint-usesamecolorasborder/">UseSameColorAsBorder</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2specialcombadditionalstylesint/">2DAdditionalStyles</a>.<a href="../../properties/irepd2specialcombadditionalstylesint-filling/">Filling</a> | <a href="../irepd2shapeobjbarshorizontalsettingsint/">2DBarsHorizontalSettings</a>.<a href="../../properties/irepd2shapeobjbarshorizontalsettingsint-filling/">Filling</a> | <a href="../irepd2shapeobjbarssettingsint/">2DBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarssettingsint-filling/">Filling</a> | <a href="../irepd2shapeobjdifferentialsettingsint/">2DDifferentialSettings</a>.<a href="../../properties/irepd2shapeobjdifferentialsettingsint-filling/">Filling</a> | <a href="../irepd2shapeobjbarsgroupedsettingsint/">2DGroupedBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-filling/">Filling</a> | <a href="../irepd2shapeobjbarsstackedsettingsint/">2DStackedBarsSettings</a>.<a href="../../properties/irepd2shapeobjbarsstackedsettingsint-filling/">Filling</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2BarFillingInt.htm`*

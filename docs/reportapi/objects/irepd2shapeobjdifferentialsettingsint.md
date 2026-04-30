---
title: "IRepD2ShapeObjDifferentialSettingsInt"
description: "The 2DDifferentialSettings object provides the curve parameter properties of a 2D axis system in the Differential display mode in DIAdem REPORT."
---

# IRepD2ShapeObjDifferentialSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DDifferentialSettings

The 2DDifferentialSettings object provides the curve parameter properties of a 2D axis system in the Differential display mode in DIAdem REPORT.

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeDifferential, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.YChannelDifferential.Reference = "[2]/[3]"
oMySettings = oMyShape.Settings
oMySettings.Type = dd.e2DDifferentialRange
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMySettings.BorderLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjdifferentialsettingsint-borderline/">BorderLine</a> | <a href="../../properties/irepd2shapeobjdifferentialsettingsint-filling/">Filling</a> | <a href="../../properties/irepd2shapeobjdifferentialsettingsint-horizontaloffset/">HorizontalOffset</a> | <a href="../../properties/irepd2shapeobjdifferentialsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjdifferentialsettingsint-type/">Type</a> | <a href="../../properties/irepd2shapeobjdifferentialsettingsint-usecurveexpansion/">UseCurveExpansion</a> | <a href="../../properties/irepd2shapeobjdifferentialsettingsint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjdifferentialint/">2DDifferential</a>.<a href="../../properties/irepd2shapeobjdifferentialint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjDifferentialSettingsInt.htm`*

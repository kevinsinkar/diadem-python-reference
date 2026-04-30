---
title: "IRepD2ShapeObjBarsStackedSettingsInt"
description: "The 2DStackedBarsSettings object provides the properties of the curve parameters of a 2D axis system in the Stacked bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsStackedSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DStackedBarsSettings

The 2DStackedBarsSettings object provides the properties of the curve parameters of a 2D axis system in the Stacked bars display mode in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeStackedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Add("[4]/[3]")

oMySettings = oMy2DCurve.Shape.Settings
oMySettings.DisplayMode = dd.eBarsDisplayMode3D
oMySettings.Mode = dd.eBarsStackModePhysical

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjbarsstackedsettingsint-borderline/">BorderLine</a> | <a href="../../properties/irepd2shapeobjbarsstackedsettingsint-displaymode/">DisplayMode</a> | <a href="../../properties/irepd2shapeobjbarsstackedsettingsint-filling/">Filling</a> | <a href="../../properties/irepd2shapeobjbarsstackedsettingsint-mode/">Mode</a> | <a href="../../properties/irepd2shapeobjbarsstackedsettingsint-offset/">Offset</a> | <a href="../../properties/irepd2shapeobjbarsstackedsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjbarsstackedsettingsint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjbarsstackedint/">2DStackedBars</a>.<a href="../../properties/irepd2shapeobjbarsstackedint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBarsStackedSettingsInt.htm`*

---
title: "IRepD2ShapeObjBarsGroupedSettingsInt"
description: "The 2DGroupedBarsSettings object provides the properties of the curve parameters of a 2D axis system in the Bars display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBarsGroupedSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DGroupedBarsSettings

The 2DGroupedBarsSettings object provides the properties of the curve parameters of a 2D axis system in the Bars display mode in DIAdem REPORT.

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

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeGroupedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Add("[4]/[3]")

oMySettings = oMy2DCurve.Shape.Settings
oMySettings.DisplayMode = dd.eBarsDisplayMode3D

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-borderline/">BorderLine</a> | <a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-displaymode/">DisplayMode</a> | <a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-filling/">Filling</a> | <a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-groupspace/">GroupSpace</a> | <a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-palette/">Palette</a> | <a href="../../properties/irepd2shapeobjbarsgroupedsettingsint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2shapeobjbarsgroupedint/">2DGroupedBars</a>.<a href="../../properties/irepd2shapeobjbarsgroupedint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ShapeObjBarsGroupedSettingsInt.htm`*

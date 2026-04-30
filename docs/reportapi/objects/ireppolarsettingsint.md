---
title: "IRepPolarSettingsInt"
description: "The PolarSectors object provides general properties of a polar axis system in DIAdem REPORT."
---

# IRepPolarSettingsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarSettings

The PolarSectors object provides general properties of a polar axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.Position.ByCoordinate.X1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.Y1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.X2 = 80
oMyPolarAxisSystem.Position.ByCoordinate.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarAxisSystem.RadialAxis.Scaling.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarAxisSystem.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow )
oMyPolarAxisSystem.Settings.HideSectorLinesInCenter = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarsettingsint-backgroundcolor/">BackgroundColor</a> | <a href="../../properties/ireppolarsettingsint-hidesectorlinesincenter/">HideSectorLinesInCenter</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarint/">PolarSystem</a>.<a href="../../properties/ireppolarint-settings/">Settings</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarSettingsInt.htm`*

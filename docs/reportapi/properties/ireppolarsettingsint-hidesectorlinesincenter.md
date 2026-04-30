---
title: "IRepPolarSettingsInt.HideSectorLinesInCenter"
description: "Specifies whether DIAdem displays the sectors of the polar axis system from the beginning of the radial axis or from the center point of the radial axis."
---

# IRepPolarSettingsInt.HideSectorLinesInCenter

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: HideSectorLinesInCenter for PolarSettings

Specifies whether DIAdem displays the sectors of the polar axis system from the beginning of the radial axis or from the center point of the radial axis.

## Signature

```python
obj.HideSectorLinesInCenter
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPolarAxisSystem.Position.ByCoordinate.X1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.Y1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.X2 = 80
oMyPolarAxisSystem.Position.ByCoordinate.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyPolarAxisSystem.Sectors.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSettings = oMyPolarAxisSystem.Settings
oMyPolarSettings.HideSectorLinesInCenter = True
oMyPolarSettings.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_HideSectorLinesInCenter_IRepPolarSettingsInt.htm`*

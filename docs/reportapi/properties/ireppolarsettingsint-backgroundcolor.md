---
title: "IRepPolarSettingsInt.BackgroundColor"
description: "Specifies the background color of a polar axis system in DIAdem REPORT."
---

# IRepPolarSettingsInt.BackgroundColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundColor for PolarSettings

Specifies the background color of a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundColor
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
OMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
OMyCurve.Shape.XChannel.Reference = "[5]/[1]"
OMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarAxisSystem.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow )
oMyPolarAxisSystem.Settings.HideSectorLinesInCenter = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundColor_IRepPolarSettingsInt.htm`*

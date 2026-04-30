---
title: "IRepPolarShapeObjLineAndPointsInt.Settings"
description: "Specifies the extended properties of a curve in the Line and points display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjLineAndPointsInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for PolarLineAndPoints

Specifies the extended properties of a curve in the Line and points display mode in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "PolarSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMySettings = oMyCurve.Shape.Settings
oMySettings.Line.LineType = dd.eLineTypeDashDot
oMySettings.Points.RelativePosition = dd.eRelativePositionPointLeftBottom
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepPolarShapeObjLineAndPointsInt.htm`*

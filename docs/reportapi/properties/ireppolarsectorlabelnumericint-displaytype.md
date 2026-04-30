---
title: "IRepPolarSectorLabelNumericInt.DisplayType"
description: "Specifies whether DIAdem REPORT displays only positive angles (0 ° to 360 or 0 to 2 Pi) or positive and negative angles (-180 ° to 180 ° or -Pi to Pi), in a plo"
---

# IRepPolarSectorLabelNumericInt.DisplayType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DisplayType for PolarSectorNumbers

Specifies whether DIAdem REPORT displays only positive angles (0 ° to 360 or 0 to 2 Pi) or positive and negative angles (-180 ° to 180 ° or -Pi to Pi), in a plor axis system.

## Signature

```python
obj.DisplayType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eDisplayTypePositive` | 0 | Positive angles |
| `eDisplayTypePositiveAndNegative` | 1 | Positive and negative angles |

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
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSectorNumbers = oMyPolarSector.Numbers
oMyPolarSectorNumbers.Font.Bold = True
oMyPolarSectorNumbers.AngleUnit = dd.eAngleUnitDegree
oMyPolarSectorNumbers.Angle = 45
oMyPolarSectorNumbers.DisplayType = dd.eDisplayTypePositiveAndNegative
oMyPolarSectorNumbers.Font.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DisplayType_IRepPolarSectorLabelNumericInt.htm`*

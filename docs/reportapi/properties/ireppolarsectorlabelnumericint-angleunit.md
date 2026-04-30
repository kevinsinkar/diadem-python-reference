---
title: "IRepPolarSectorLabelNumericInt.AngleUnit"
description: "Specifies whether DIAdem REPORT displays the circle labels of the polar axis system in degrees or in radians."
---

# IRepPolarSectorLabelNumericInt.AngleUnit

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AngleUnit for PolarSectorNumbers

Specifies whether DIAdem REPORT displays the circle labels of the polar axis system in degrees or in radians.

## Signature

```python
obj.AngleUnit
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngleUnitDegree` | 0 | Degree |
| `eAngleUnitRad` | 1 | Radian |

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPolarAxisSystem.Position.ByCoordinate.X1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.Y1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.X2 = 80
oMyPolarAxisSystem.Position.ByCoordinate.Y2 = 80
OMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
OMyCurve.Shape.XChannel.Reference = "[5]/[1]"
OMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSectorNumbers = oMyPolarSector.Numbers
oMyPolarSectorNumbers.Font.Bold = True
oMyPolarSectorNumbers.AngleUnit = dd.eAngleUnitDegree
oMyPolarSectorNumbers.Angle = 45
oMyPolarSectorNumbers.Font.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AngleUnit_IRepPolarSectorLabelNumericInt.htm`*

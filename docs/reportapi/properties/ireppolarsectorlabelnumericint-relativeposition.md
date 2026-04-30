---
title: "IRepPolarSectorLabelNumericInt.RelativePosition"
description: "Specifies the relative position of the circle numbers of a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorLabelNumericInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for PolarSectorNumbers

Specifies the relative position of the circle numbers of a polar axis system in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionRightTop` | 0 | Top right |
| `eRelativePositionCenter` | 1 | Center |
| `eRelativePositionRight` | 2 | Right |
| `eRelativePositionRightBottom` | 3 | Bottom right |
| `eRelativePositionTop` | 4 | Top |
| `eRelativePositionBottom` | 5 | Bottom |
| `eRelativePositionLeftTop` | 6 | Top left |
| `eRelativePositionLeft` | 7 | Left |
| `eRelativePositionLeftBottom` | 8 | Bottom left |
| `eRelativePositionNumericLabelAutomatic` | 12 | Automatic |

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
oMyPolarSectorNumbers.RelativePosition = dd.eRelativePositionLeft
oMyPolarSectorNumbers.Font.Bold = True
oMyPolarSectorNumbers.AngleUnit = dd.eAngleUnitDegree
oMyPolarSectorNumbers.Angle = 45
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

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepPolarSectorLabelNumericInt.htm`*

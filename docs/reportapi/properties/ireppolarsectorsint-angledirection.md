---
title: "IRepPolarSectorsInt.AngleDirection"
description: "Specifies the direction of the circle labeling of a polar axis system in DIAdem REPORT. DIAdem only includes the property AngleDirection if you assign the value"
---

# IRepPolarSectorsInt.AngleDirection

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AngleDirection for PolarSectors

Specifies the direction of the circle labeling of a polar axis system in DIAdem REPORT. DIAdem only includes the property AngleDirection if you assign the value eAxisScalingSimpleManual to the AutoScalingType property.

## Signature

```python
obj.AngleDirection
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAngleDirectionCounterClockwise` | 0 | Counter clockwise |
| `eAngleDirectionClockwise` | 1 | Clockwise |

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
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSector.SectorCount = 8
oMyPolarSector.AngleDirection = dd.eAngleDirectionClockwise
oMyPolarSector.MiniSectorCount = 7
oMyPolarSector.MiniSectorLine.LineType = dd.eLineTypeDashed1
oMyPolarSector.MiniSectorStartIndex = 2
oMyPolarSector.Numbers.Format = "d"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AngleDirection_IRepPolarSectorsInt.htm`*

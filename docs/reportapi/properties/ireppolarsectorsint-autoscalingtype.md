---
title: "IRepPolarSectorsInt.AutoScalingType"
description: "Specifies whether DIAdem REPORT scales the sectors of a polar axis system automatically."
---

# IRepPolarSectorsInt.AutoScalingType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AutoScalingType for PolarSectors

Specifies whether DIAdem REPORT scales the sectors of a polar axis system automatically.

## Signature

```python
obj.AutoScalingType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisScalingSimpleManual` | 0 | Manual |
| `eAxisScalingSimpleCompleteAutomatic` | 1 | Fully automatic |
| `eAxisAutoScalingCustom` | 2 | User-defined axis scaling |

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

*Source: `ReportApi/properties/Report_property_AutoScalingType_IRepPolarSectorsInt.htm`*

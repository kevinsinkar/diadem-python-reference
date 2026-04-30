---
title: "IRepPolarSectorsInt.MiniSectorStartIndex"
description: "Specifies the number of the circle on the radial axis at which DIAdem starts dividing the circle sectors into minisectors in the polar axis system in DIAdem REP"
---

# IRepPolarSectorsInt.MiniSectorStartIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MiniSectorStartIndex for PolarSectors

Specifies the number of the circle on the radial axis at which DIAdem starts dividing the circle sectors into minisectors in the polar axis system in DIAdem REPORT. The numbering starts in the center of the circle. DIAdem only includes the property MiniSectorStartIndex if you assign the value eAxisScalingSimpleManual to the AutoScalingType property.

## Signature

```python
obj.MiniSectorStartIndex
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
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MiniSectorStartIndex_IRepPolarSectorsInt.htm`*

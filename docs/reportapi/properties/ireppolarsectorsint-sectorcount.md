---
title: "IRepPolarSectorsInt.SectorCount"
description: "Specifies the number of sectors in a polar axis system in DIAdem REPORT. Assign the value eAxisScalingSimpleManual to the property AutoScalingType if you want t"
---

# IRepPolarSectorsInt.SectorCount

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SectorCount for PolarSectors

Specifies the number of sectors in a polar axis system in DIAdem REPORT. Assign the value eAxisScalingSimpleManual to the property AutoScalingType if you want to specify the start value manually.

## Signature

```python
obj.SectorCount
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
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSector.SectorCount = 8
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SectorCount_IRepPolarSectorsInt.htm`*

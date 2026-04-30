---
title: "IRepPolarSectorsInt.SectorLine"
description: "Specifies the properties of the sector boundary lines in a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorsInt.SectorLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: SectorLine for PolarSectors

Specifies the properties of the sector boundary lines in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.SectorLine
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
oMyPolarSector.SectorLine.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMyPolarSector.SectorLine.LineType = dd.eLineTypeSolid
oMyPolarSector.SectorLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_SectorLine_IRepPolarSectorsInt.htm`*

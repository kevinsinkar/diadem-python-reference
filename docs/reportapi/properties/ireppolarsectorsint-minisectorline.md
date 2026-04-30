---
title: "IRepPolarSectorsInt.MiniSectorLine"
description: "Specifies the line properties of the of the mini sectors in a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorsInt.MiniSectorLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MiniSectorLine for PolarSectors

Specifies the line properties of the of the mini sectors in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.MiniSectorLine
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
OMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
OMyCurve.Shape.XChannel.Reference = "[5]/[1]"
OMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSector.SectorCount = 8
oMyPolarSector.AngleDirection = dd.eAngleDirectionClockwise
oMyPolarSector.MiniSectorCount = 7
oMyPolarSector.MiniSectorLine.LineType = dd.eLineTypeDashed1
oMyPolarSector.MiniSectorLine.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMyPolarSector.MiniSectorLine.Interval = 1
oMyPolarSector.MiniSectorLine.Width = dd.eLineWidth0025
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MiniSectorLine_IRepPolarSectorsInt.htm`*

---
title: "IRepPolarSectorLabelNumericInt.Format"
description: "Specifies the Format definition of the sector labels in a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorLabelNumericInt.Format

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Format for PolarSectorNumbers

Specifies the Format definition of the sector labels in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Format
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
OMyCurve.Shape.XChannel.Reference = "[5]/[1]"
OMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSectorNumbers = oMyPolarSector.Numbers
oMyPolarSectorNumbers.Format = "d.dd"
oMyPolarSectorNumbers.Font.Bold = True
oMyPolarSectorNumbers.Font.Name = "Arial"
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

*Source: `ReportApi/properties/Report_property_Format_IRepPolarSectorLabelNumericInt.htm`*

---
title: "IRepPolarSectorsInt.Numbers"
description: "Specifies the properties of the circle numbers of a polar axis system in DIAdem REPORT."
---

# IRepPolarSectorsInt.Numbers

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Numbers for PolarSectors

Specifies the properties of the circle numbers of a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Numbers
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSector = oMyPolarAxisSystem.Sectors
oMyPolarSector.Numbers.Angle = "45"
oMyPolarSector.Numbers.Font.Name = "Times Roman"()
oMyPolarSector.Numbers.Font.Size = 3
oMyPolarSector.Numbers.Format = "d.d"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Numbers_IRepPolarSectorsInt.htm`*

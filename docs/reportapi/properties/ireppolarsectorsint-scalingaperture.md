---
title: "IRepPolarSectorsInt.ScalingAperture"
description: "Specifies the aperture angle of a sector in degrees in a polar axis system in DIAdem REPORT. Assign the value eAxisScalingSimpleManual to the property AutoScali"
---

# IRepPolarSectorsInt.ScalingAperture

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ScalingAperture for PolarSectors

Specifies the aperture angle of a sector in degrees in a polar axis system in DIAdem REPORT. Assign the value eAxisScalingSimpleManual to the property AutoScalingType if you want to specify the aperture angle manually.

## Signature

```python
obj.ScalingAperture
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
oMyPolarSector.AutoScalingType = dd.eAxisScalingSimpleManual
oMyPolarSector.ScalingAperture = "330"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ScalingAperture_IRepPolarSectorsInt.htm`*

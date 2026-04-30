---
title: "IRepPolarSectorsInt.ScalingZeroAngle"
description: "Specifies the zero angle alignment of the radial axis in a polar axis system in degrees in DIAdem REPORT. Assign the value eAxisScalingSimpleManual to the prope"
---

# IRepPolarSectorsInt.ScalingZeroAngle

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ScalingZeroAngle for PolarSectors

Specifies the zero angle alignment of the radial axis in a polar axis system in degrees in DIAdem REPORT. Assign the value eAxisScalingSimpleManual to the property AutoScalingType if you want to specify the start value manually.

## Signature

```python
obj.ScalingZeroAngle
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
oMyPolarSector.ScalingZeroAngle = 45
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ScalingZeroAngle_IRepPolarSectorsInt.htm`*

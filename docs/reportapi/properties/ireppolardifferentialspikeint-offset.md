---
title: "IRepPolarDifferentialSpikeInt.Offset"
description: "Specifies the displacement of the upper and lower lines in the Differential curve type in a polar axis system in DIAdem REPORT."
---

# IRepPolarDifferentialSpikeInt.Offset

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Offset for PolarDifferentialDimension

Specifies the displacement of the upper and lower lines in the Differential curve type in a polar axis system in DIAdem REPORT.

## Signature

```python
obj.Offset
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 0
oMyPosition.Y1 = 0
oMyPosition.X2 = 90
oMyPosition.Y2 = 90
oMySectors = oMyPolarAxisSystem.Sectors
oMySectors.AutoScalingType = dd.eAxisScalingSimpleManual
oMySectors.ScalingAperture = 90
oMySectors.SectorCount = 3
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeDifferential, "MyCurve")
oMyCurve.Shape.XChannel.Reference = ""
oMyCurve.Shape.YChannel.Reference = "[4]/[1]"
oMyCurve.Shape.YChannelDifferential.Reference = "[4]/[2]"
oMyCurve.Shape.DifferentialLine.Color.SetPredefinedColor(dd.ePredefinedColorDarkGreen)
oMyCurve.Shape.DifferentialDimension.Offset = 10
oMyCurve.Shape.DifferentialDimension.Width = 0
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Offset_IRepPolarDifferentialSpikeInt.htm`*

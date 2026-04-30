---
title: "IRepPolarDifferentialSpikeInt.Width"
description: "Specifies the width of the upper and lower lines as a percentage of the minimum interval of the lines for the Differential curve type in a polar axis system in "
---

# IRepPolarDifferentialSpikeInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for PolarDifferentialDimension

Specifies the width of the upper and lower lines as a percentage of the minimum interval of the lines for the Differential curve type in a polar axis system in DIAdem REPORT. If these lines are very close in the middle of the circle, this interval is very small.

## Signature

```python
obj.Width
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeDifferential, "MyNewCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference= "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMyShape.YChannelDifferential.Reference = "[5]/[3]"
oMyShape.DifferentialDimension.Offset = 10
oMyShape.DifferentialDimension.Width = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepPolarDifferentialSpikeInt.htm`*

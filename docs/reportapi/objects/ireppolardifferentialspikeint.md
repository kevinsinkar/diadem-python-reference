---
title: "IRepPolarDifferentialSpikeInt"
description: "The PolarDifferentialDimension object provides the parameters of the Differential curve type in a polar axis system in DIAdem REPORT."
---

# IRepPolarDifferentialSpikeInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarDifferentialDimension

The PolarDifferentialDimension object provides the parameters of the Differential curve type in a polar axis system in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolardifferentialspikeint-offset/">Offset</a> | <a href="../../properties/ireppolardifferentialspikeint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarshapeobjdifferentialint/">PolarDifferential</a>.<a href="../../properties/ireppolarshapeobjdifferentialint-differentialdimension/">DifferentialDimension</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarDifferentialSpikeInt.htm`*

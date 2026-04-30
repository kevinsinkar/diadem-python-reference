---
title: "IRepPolarShapeObjDifferentialInt"
description: "The PolarDifferential object provides the curve properties in the Differential display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjDifferentialInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarDifferential

The PolarDifferential object provides the curve properties in the Differential display mode in a polar axis system in DIAdem REPORT.

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
oMyShape.DifferentialLine.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarshapeobjdifferentialint-differentialdimension/">DifferentialDimension</a> | <a href="../../properties/ireppolarshapeobjdifferentialint-differentialline/">DifferentialLine</a> | <a href="../../properties/ireppolarshapeobjdifferentialint-xchannel/">XChannel</a> | <a href="../../properties/ireppolarshapeobjdifferentialint-ychannel/">YChannel</a> | <a href="../../properties/ireppolarshapeobjdifferentialint-ychanneldifferential/">YChannelDifferential</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarcurveint/">PolarCurve</a>.<a href="../../properties/ireppolarcurveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarShapeObjDifferentialInt.htm`*

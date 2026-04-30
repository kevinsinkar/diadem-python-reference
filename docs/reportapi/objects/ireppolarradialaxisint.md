---
title: "IRepPolarRadialAxisInt"
description: "The PolarRadialAxis object provides the radial axis properties for a polar axis system in DIAdem REPORT."
---

# IRepPolarRadialAxisInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarRadialAxis

The PolarRadialAxis object provides the radial axis properties for a polar axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyRadialAxis = oMyPolarAxisSystem.RadialAxis
oMyRadialAxis.Label.Text = "MyRadialAxis"
oMyRadialAxis.MiniTickLine.LineType = dd.eLineTypeDotted
oMyRadialAxis.Numbers.UseCurveColor = True
oMyRadialAxis.Numbers.Format = "d.d"
oMyRadialAxis.NumbersRepetitionMode = dd.ePolarAxisNumbersEvery090
oMyRadialAxis.Scaling.Begin = 10
oMyRadialAxis.Scaling.End = 20
oMyRadialAxis.TickLine.Width = dd.eLineWidth0070
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarradialaxisint-label/">Label</a> | <a href="../../properties/ireppolarradialaxisint-minitickline/">MiniTickLine</a> | <a href="../../properties/ireppolarradialaxisint-miniticktype/">MiniTickType</a> | <a href="../../properties/ireppolarradialaxisint-numbers/">Numbers</a> | <a href="../../properties/ireppolarradialaxisint-numbersrepetitionmode/">NumbersRepetitionMode</a> | <a href="../../properties/ireppolarradialaxisint-scaling/">Scaling</a> | <a href="../../properties/ireppolarradialaxisint-tickline/">TickLine</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarint/">PolarSystem</a>.<a href="../../properties/ireppolarint-radialaxis/">RadialAxis</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarRadialAxisInt.htm`*

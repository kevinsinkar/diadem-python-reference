---
title: "IRepCurveLegendInt"
description: "The CurveLegend object provides the curve legend object in DIAdem REPORT."
---

# IRepCurveLegendInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CurveLegend

The CurveLegend object provides the curve legend object in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.CurveLegend.Visible = True
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcurvelegendint-columns/">Columns</a> | <a href="../../properties/irepcurvelegendint-frame/">Frame</a> | <a href="../../properties/irepcurvelegendint-header/">Header</a> | <a href="../../properties/irepcurvelegendint-position/">Position</a> | <a href="../../properties/irepcurvelegendint-settings/">Settings</a> | <a href="../../properties/irepcurvelegendint-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisint/">2DAxisSystem</a>.<a href="../../properties/irepd2axisint-curvelegend/">CurveLegend</a> | <a href="../irepd3axisint/">3DAxisSystem</a>.<a href="../../properties/irepd3axisint-curvelegend/">CurveLegend</a> | <a href="../ireppiechartint/">PieChart</a>.<a href="../../properties/ireppiechartint-legend/">Legend</a> | <a href="../ireppolarint/">PolarSystem</a>.<a href="../../properties/ireppolarint-curvelegend/">CurveLegend</a> | <a href="../irepspiderint/">Spider</a>.<a href="../../properties/irepspiderint-curvelegend/">CurveLegend</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCurveLegendInt.htm`*

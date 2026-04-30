---
title: "IRepCurvelegendContentColumnInt"
description: "The CurveLegendColumn object provides the properties of a column from the curve legend in DIAdem REPORT."
---

# IRepCurvelegendContentColumnInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: CurveLegendColumn

The CurveLegendColumn object provides the properties of a column from the curve legend in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNewCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DaxisSystem.CurveLegend.Visible = True
oMyLegendColumn = oMy2DaxisSystem.CurveLegend.Columns.Add()
oMyLegendColumn.Type = dd.eLegendTextComment
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepcurvelegendcontentcolumnint-relativewidth/">RelativeWidth</a> | <a href="../../properties/irepcurvelegendcontentcolumnint-text/">Text</a> | <a href="../../properties/irepcurvelegendcontentcolumnint-title/">Title</a> | <a href="../../properties/irepcurvelegendcontentcolumnint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/curvelegendcolumns/">CurveLegendColumns</a>.<a href="../../methods/irepcurvelegendcontentcolumnslistint-add/">Add</a> | <a href="../../collections/curvelegendcolumns/">CurveLegendColumns</a>.<a href="../../methods/irepcurvelegendcontentcolumnslistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepCurvelegendContentColumnInt.htm`*

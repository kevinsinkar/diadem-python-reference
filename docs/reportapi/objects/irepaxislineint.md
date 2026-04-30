---
title: "IRepAxisLineInt"
description: "The AxisLine object provides the line properties of an axis in a 2D axis system in DIAdem REPORT."
---

# IRepAxisLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: AxisLine

The AxisLine object provides the line properties of an axis in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXLine = oMy2DAxisSystem.XAxis.Line
oMyXLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyXLine.UseCurveColor = False
oMyXLine.Width = dd.eLineWidth0100
oMyYLine = oMy2DAxisSystem.YAxis.Line
oMyYLine.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyYLine.UseCurveColor = False
oMyYLine.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepaxislineint-color/">Color</a> | <a href="../../properties/irepaxislineint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepaxislineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2axisxint/">2DAxisX</a>.<a href="../../properties/irepd2axisxint-line/">Line</a> | <a href="../irepd2axisyint/">2DAxisY</a>.<a href="../../properties/irepd2axisyint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepAxisLineInt.htm`*

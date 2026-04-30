---
title: "IRepD2ErrorBarLineInt"
description: "The 2DErrorBarLine object provides the curve parameters of an error bar in a 2D axis system in DIAdem REPORT."
---

# IRepD2ErrorBarLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: 2DErrorBarLine

The 2DErrorBarLine object provides the curve parameters of an error bar in a 2D axis system in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "examples\\Data\\Error_Bars.tdm","TDM","")
dd.Report.NewLayout()
oMyReportObj = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMyReportObj.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyReportObj.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyErrorBars = oMyShape.Extensions.ErrorBars
oMyErrorBars.XErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyErrorBars.XErrorBar.PercentageErrorValue = 10
oMyErrorBars.Line.UseCurveColor = False
oMyErrorBars.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepd2errorbarlineint-color/">Color</a> | <a href="../../properties/irepd2errorbarlineint-interval/">Interval</a> | <a href="../../properties/irepd2errorbarlineint-linetype/">LineType</a> | <a href="../../properties/irepd2errorbarlineint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepd2errorbarlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2errorbarsadditionalint/">2DAdditionalErrorBars</a>.<a href="../../properties/irepd2errorbarsadditionalint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepD2ErrorBarLineInt.htm`*

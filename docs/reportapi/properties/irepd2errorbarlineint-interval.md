---
title: "IRepD2ErrorBarLineInt.Interval"
description: "Specifies the line interval of broken lines when displaying an error bar in a 2D axis system in DIAdem REPORT. Greater values mean greater intervals."
---

# IRepD2ErrorBarLineInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for 2DErrorBarLine

Specifies the line interval of broken lines when displaying an error bar in a 2D axis system in DIAdem REPORT. Greater values mean greater intervals.

## Signature

```python
obj.Interval
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "examples\\Data\\Error_Bars.tdm","TDM","")
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
oMyErrorBars.Line.UseCurveColor = False
oMyErrorBars.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMyErrorBars.Line.LineType = dd.eLineTypeDotted
oMyErrorBars.Line.Interval = 1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepD2ErrorBarLineInt.htm`*

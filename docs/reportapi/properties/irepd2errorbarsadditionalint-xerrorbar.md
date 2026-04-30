---
title: "IRepD2ErrorBarsAdditionalInt.XErrorBar"
description: "Returns an error bar in x direction in a 2D axis system in DIAdem REPORT."
---

# IRepD2ErrorBarsAdditionalInt.XErrorBar

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: XErrorBar for 2DAdditionalErrorBars

Returns an error bar in x direction in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.XErrorBar
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
oMyErrorBars.XErrorBar.ErrorType= dd.eErrorbarErrorTypePercentage
oMyErrorBars.XErrorBar.PercentageErrorValue = 15
oMyErrorBars.Line.UseCurveColor = False
oMyErrorBars.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
oMyErrorBars.Line.LineType = dd.eLineTypeSolid
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_XErrorBar_IRepD2ErrorBarsAdditionalInt.htm`*

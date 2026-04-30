---
title: "IRepErrorBarInt.AbsoluteErrorValue"
description: "Specifies the absolute error value of a 2D curve with error bars in DIAdem REPORT."
---

# IRepErrorBarInt.AbsoluteErrorValue

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: AbsoluteErrorValue for ErrorBar

Specifies the absolute error value of a 2D curve with error bars in DIAdem REPORT.

## Signature

```python
obj.AbsoluteErrorValue
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[6]/[1]"
oMyCurve.Shape.YChannel.Reference = "[6]/[2]"
oMyErrorBars = oMyCurve.Shape.Extensions.ErrorBars
oMyErrorBars.YErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyErrorBars.YErrorBar.ErrorType = dd.eErrorbarErrorTypeAbsoluteError
oMyErrorBars.YErrorBar.AbsoluteErrorValue = 2
oMyErrorBars.Line.LineType = dd.eLineTypeSolid
oMyErrorBars.EndCap.Type = dd.eErrorbarDisplaySpike
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_AbsoluteErrorValue_IRepErrorBarInt.htm`*

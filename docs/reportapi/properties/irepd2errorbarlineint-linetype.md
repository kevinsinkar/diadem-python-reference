---
title: "IRepD2ErrorBarLineInt.LineType"
description: "Specifies the line style of an error bar in a 2D axis system in DIAdem REPORT."
---

# IRepD2ErrorBarLineInt.LineType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineType for 2DErrorBarLine

Specifies the line style of an error bar in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.LineType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineTypeNone` | 0 | None |
| `eLineTypeSolid` | 1 | Line |
| `eLineTypeDashDot` | 2 | Dots and dashes |
| `eLineTypeDashed1` | 3 | Dashes 1 |
| `eLineTypeDashed2` | 4 | Dashes 2 |
| `eLineTypeDotted` | 5 | Dotted |

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
oMyErrorBars.EndCap.Type = dd.eErrorbarDisplaySpike
oMyErrorBarsLine = oMyErrorBars.Line
oMyErrorBarsLine.LineType = dd.eLineTypeSolid
oMyErrorBarsLine.UseCurveColor = False
oMyErrorBarsLine.Color.SetPredefinedColor(dd.ePredefinedColorTurquoise)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LineType_IRepD2ErrorBarLineInt.htm`*

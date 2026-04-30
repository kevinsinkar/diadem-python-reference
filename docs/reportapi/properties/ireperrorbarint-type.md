---
title: "IRepErrorBarInt.Type"
description: "Specifies the direction of the error bars in a 2D axis system in DIAdem REPORT."
---

# IRepErrorBarInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for ErrorBar

Specifies the direction of the error bars in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eErrorbarNone` | 0 | None |
| `eErrorbarPositiveAndNegative` | 1 | Both sides |
| `eErrorbarPositive` | 2 | Positive |
| `eErrorbarNegative` | 3 | Negative |

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
oMyCurve.Shape.Extensions.ErrorBars.YErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyCurve.Shape.Extensions.ErrorBars.YErrorBar.PercentageErrorValue = 10
oMyCurve.Shape.Extensions.ErrorBars.EndCap.Type = dd.eErrorbarDisplaySpike
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepErrorBarInt.htm`*

---
title: "IRepD2ErrorBarLineInt.UseCurveColor"
description: "Specifies whether DIAdem REPORT displays the error bars of a 2D axis system in the same color as the curve."
---

# IRepD2ErrorBarLineInt.UseCurveColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseCurveColor for 2DErrorBarLine

Specifies whether DIAdem REPORT displays the error bars of a 2D axis system in the same color as the curve.

## Signature

```python
obj.UseCurveColor
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "\\examples\\data\\Error_Bars.tdm","tdm","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyShape.Extensions.ErrorBars.XErrorBar.Type = dd.eErrorbarPositiveAndNegative
oMyShape.Extensions.ErrorBars.XErrorBar.PercentageErrorValue = 10
oMyShape.Extensions.ErrorBars.Line.UseCurveColor = False
oMyShape.Extensions.ErrorBars.Line.Color.SetPredefinedColor(dd.eColorIndexGreen)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_UseCurveColor_IRepD2ErrorBarLineInt.htm`*

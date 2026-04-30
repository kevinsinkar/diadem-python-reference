---
title: "IRepD2ShapeObjLineAndPointsExtensionsInt.ErrorBars"
description: "Returns an error bar for the curve type Line and points in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjLineAndPointsExtensionsInt.ErrorBars

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ErrorBars for 2DLineAndPointsExtensions

Returns an error bar for the curve type Line and points in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.ErrorBars
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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
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
oMyMarker = oMyCurve.Shape.Extensions.Marker
oMyMarker.Type = dd.eMarkerCircle
oMyMarker.Size = 3
oMyMarker.Repetition.Mode = dd.eMarkerRepetitionMaximalNPoints
oMyMarker.Repetition.NValue = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ErrorBars_IRepD2ShapeObjLineAndPointsExtensionsInt.htm`*

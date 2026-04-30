---
title: "IRepLineFullFeaturedInt.Interval"
description: "Specifies the line interval for broken lines in an axis system in DIAdem REPORT. Greater values mean greater intervals."
---

# IRepLineFullFeaturedInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for FullFeaturedLine

Specifies the line interval for broken lines in an axis system in DIAdem REPORT. Greater values mean greater intervals.

## Signature

```python
obj.Interval
```

## Python example

```python
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyRadialAxis = oMyPolarAxisSystem.RadialAxis
oMyRadialAxis.Label.Text = "MyRadialAxis"
oMyRadialAxis.MiniTickLine.LineType = dd.eLineTypeDashDot
oMyRadialAxis.MiniTickLine.Interval = 4
oMyRadialAxis.Numbers.UseCurveColor = True
oMyRadialAxis.Numbers.Format = "d.d"
oMyRadialAxis.NumbersRepetitionMode = dd.ePolarAxisNumbersEvery090
oMyRadialAxis.Scaling.Begin = 10
oMyRadialAxis.Scaling.End = 20
oMyRadialAxis.TickLine.Width = dd.eLineWidth0070
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepLineFullFeaturedInt.htm`*

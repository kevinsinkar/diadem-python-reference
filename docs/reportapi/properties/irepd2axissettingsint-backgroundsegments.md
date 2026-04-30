---
title: "IRepD2AxisSettingsInt.BackgroundSegments"
description: "Specifies the background segments of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisSettingsInt.BackgroundSegments

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BackgroundSegments for 2DAxisSettings

Specifies the background segments of a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.BackgroundSegments
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.ProgramDrv + "examples\\data\\Segment.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMySegement = oMy2DAxisSystem.Settings.BackgroundSegments.Add()
oMySegement.Color.SetPredefinedColor(dd.eColorIndexYellow)
oMySegement.XChannel.Reference = "[1]/[3]"
oMySegement.YChannel.Reference = "[1]/[4]"
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_BackgroundSegments_IRepD2AxisSettingsInt.htm`*

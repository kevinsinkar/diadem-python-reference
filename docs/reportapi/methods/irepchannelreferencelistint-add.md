---
title: "IRepChannelReferenceListInt.Add"
description: "Adds a new y-channel to a 2D axis system in the display mode Stacked Bars or Grouped Bars in DIAdem-REPORT."
---

# IRepChannelReferenceListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for Channels

Adds a new y-channel to a 2D axis system in the display mode Stacked Bars or Grouped Bars in DIAdem-REPORT.

## Signature

```python
return_value = obj.Add(Reference)
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")

oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeStackedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Add("[4]/[3]")

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepChannelReferenceListInt.htm`*

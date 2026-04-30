---
title: "IRepChannelReferenceListInt.Move"
description: "Moves a y-channel to a 2D axis system in the display mode Stacked Bars or Grouped Bars in DIAdem-REPORT to a different position."
---

# IRepChannelReferenceListInt.Move

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Move for Channels

Moves a y-channel to a 2D axis system in the display mode Stacked Bars or Grouped Bars in DIAdem-REPORT to a different position.

## Signature

```python
obj.Move(IndexFrom, IndexTo)
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeGroupedBars, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = ""

oMyChn1 = oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMyChn2 = oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMyChn3 = oMy2DCurve.Shape.YChannels.Add("[4]/[3]")
oMyChns = oMy2DCurve.Shape.YChannels
oMyChns.Move(2,1)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Move_IRepChannelReferenceListInt.htm`*

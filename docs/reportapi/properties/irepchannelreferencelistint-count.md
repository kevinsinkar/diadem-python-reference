---
title: "IRepChannelReferenceListInt.Count"
description: "Returns the number of y-channels of a 2D axis system in the display mode Stacked bars or Grouped bars in DIAdem REPORT."
---

# IRepChannelReferenceListInt.Count

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Count for Channels

Returns the number of y-channels of a 2D axis system in the display mode Stacked bars or Grouped bars in DIAdem REPORT.

## Signature

```python
obj.Count
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
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Add("[4]/[3]")

for I in range( 1, oMy2DCurve.Shape.YChannels.Count+1):
    oMy2DCurve.Shape.Settings.Palette.Colors(I).ColorIndex = (I % 16) + 1

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Count_IRepChannelReferenceListInt.htm`*

---
title: "IRepChannelReferenceListInt.Copy"
description: "Copies in DIAdem REPORT the existing y-channel of a 2D axis system in the display mode Stacked bars or Grouped bars and adds this channel to the axis system."
---

# IRepChannelReferenceListInt.Copy

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Copy for Channels

Copies in DIAdem REPORT the existing y-channel of a 2D axis system in the display mode Stacked bars or Grouped bars and adds this channel to the axis system.

## Signature

```python
return_value = obj.Copy(Index, IndexTo)
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeGroupedBars, "MyNew2DCurve1")
oMy2DCurve.Shape.XChannel.Reference = ""
oMy2DCurve.Shape.YChannels.Add("[4]/[1]")
oMy2DCurve.Shape.YChannels.Add("[4]/[2]")
oMy2DCurve.Shape.YChannels.Copy(1,2)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Copy_IRepChannelReferenceListInt.htm`*

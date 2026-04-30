---
title: "IRepChannelRefListItemInt"
description: "The ChannelReferenceListItem object provides a y-channel in a 2D axis system in the display mode Grouped bars or Stacked bars in DIAdem REPORT."
---

# IRepChannelRefListItemInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: ChannelReferenceListItem

The ChannelReferenceListItem object provides a y-channel in a 2D axis system in the display mode Grouped bars or Stacked bars in DIAdem REPORT.

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

oMySettings = oMy2DCurve.Shape.Settings
oMySettings.BorderLine.LineType = dd.eLineTypeDashed1
oMySettings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepchannelreflistitemint-index/">Index</a> | <a href="../../properties/irepchannelreflistitemint-reference/">Reference</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../collections/channels/">Channels</a>.<a href="../../methods/irepchannelreferencelistint-add/">Add</a> | <a href="../../collections/channels/">Channels</a>.<a href="../../methods/irepchannelreferencelistint-copy/">Copy</a> | <a href="../../collections/channels/">Channels</a>.<a href="../../methods/irepchannelreferencelistint-item/">Item</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepChannelRefListItemInt.htm`*

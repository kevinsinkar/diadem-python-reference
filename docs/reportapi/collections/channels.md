---
title: "Channels"
description: "The Channels object provides the y-channels of a 2D axis system in the display mode Stacked bars or Grouped bars in DIAdem REPORT."
---

# Channels

!!! abstract "Collection &middot; `ReportApi.chm`"
    Collection: Channels

The Channels object provides the y-channels of a 2D axis system in the display mode Stacked bars or Grouped bars in DIAdem REPORT.

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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepchannelreferencelistint-count/">Count</a></p>
</div>
<div class="Methods"><h2>Methods</h2>
<p><a href="../../methods/irepchannelreferencelistint-add/">Add</a> | <a href="../../methods/irepchannelreferencelistint-copy/">Copy</a> | <a href="../../methods/irepchannelreferencelistint-item/">Item</a> | <a href="../../methods/irepchannelreferencelistint-move/">Move</a> | <a href="../../methods/irepchannelreferencelistint-remove/">Remove</a> | <a href="../../methods/irepchannelreferencelistint-removeall/">RemoveAll</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../../objects/irepd2shapeobjboxwhiskerint/">2DBoxWhisker</a>.<a href="../../properties/irepd2shapeobjboxwhiskerint-ychannels/">YChannels</a> | <a href="../../objects/irepd2shapeobjbarsgroupedint/">2DGroupedBars</a>.<a href="../../properties/irepd2shapeobjbarsgroupedint-ychannels/">YChannels</a> | <a href="../../objects/irepd2shapeobjbarsstackedint/">2DStackedBars</a>.<a href="../../properties/irepd2shapeobjbarsstackedint-ychannels/">YChannels</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepChannelReferenceListInt.htm`*

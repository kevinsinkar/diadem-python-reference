---
title: "IRepChannelRefListItemInt.Reference"
description: "Specifies the reference to a y-channel in a 2D axis system in the Grouped bars or Stacked bars display type in DIAdem-REPORT."
---

# IRepChannelRefListItemInt.Reference

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Reference for ChannelReferenceListItem

Specifies the reference to a y-channel in a 2D axis system in the Grouped bars or Stacked bars display type in DIAdem-REPORT.

## Signature

```python
obj.Reference
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

for YChannel in oMy2DCurve.Shape.YChannels:
    print("Channel index: " + YChannel.Index + "\r\n" + "Channel reference: " + YChannel.Reference)

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Reference_IRepChannelRefListItemInt.htm`*

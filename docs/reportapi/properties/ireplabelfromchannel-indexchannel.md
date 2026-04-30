---
title: "IRepLabelFromChannel.IndexChannel"
description: "Specifies the channel from which DIAdem REPORT takes the labels for a curve."
---

# IRepLabelFromChannel.IndexChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: IndexChannel for LabelFromChannel

Specifies the channel from which DIAdem REPORT takes the labels for a curve.

## Signature

```python
return_value = obj.IndexChannel
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
oMyChnLabel = oMyCurve.Shape.Extensions.Label.FromChannel
oMyChnLabel.Channel.Reference = "[7]/[1]"
oMyChnLabel.Visible = True
oMyChnLabel.IndexChannel.Reference = "[6]/[3]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_IndexChannel_IRepLabelFromChannel.htm`*

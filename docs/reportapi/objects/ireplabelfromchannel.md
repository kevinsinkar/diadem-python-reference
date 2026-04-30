---
title: "IRepLabelFromChannel"
description: "The LabelFromChannel object provides the label channel properties of a curve in DIAdem REPORT."
---

# IRepLabelFromChannel

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: LabelFromChannel

The LabelFromChannel object provides the label channel properties of a curve in DIAdem REPORT.

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
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

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireplabelfromchannel-channel/">Channel</a> | <a href="../../properties/ireplabelfromchannel-format/">Format</a> | <a href="../../properties/ireplabelfromchannel-indexchannel/">IndexChannel</a> | <a href="../../properties/ireplabelfromchannel-visible/">Visible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepd2labeladditionalint/">2DAdditionalLabel</a>.<a href="../../properties/irepd2labeladditionalint-fromchannel/">FromChannel</a> | <a href="../irepd3labelisolineadditionalint/">3DAdditionalIsolineLabel</a>.<a href="../../properties/irepd3labelisolineadditionalint-fromchannel/">FromChannel</a> | <a href="../irepd3labeladditionalint/">3DAdditionalLabel</a>.<a href="../../properties/irepd3labeladditionalint-fromchannel/">FromChannel</a> | <a href="../ireppolarlabeladditionalint/">PolarAdditionalLabel</a>.<a href="../../properties/ireppolarlabeladditionalint-fromchannel/">FromChannel</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepLabelFromChannel.htm`*

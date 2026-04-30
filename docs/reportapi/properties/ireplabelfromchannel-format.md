---
title: "IRepLabelFromChannel.Format"
description: "Specifies the Format definition for the label channel of a 2D or 3D curve in DIAdem REPORT."
---

# IRepLabelFromChannel.Format

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Format for LabelFromChannel

Specifies the Format definition for the label channel of a 2D or 3D curve in DIAdem REPORT.

## Signature

```python
obj.Format
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
oMyChnLabel.Channel.Reference = "[6]/[1]"
oMyChnLabel.Visible = True
oMyChnLabel.Format = "#HH:nn AMPM"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Format_IRepLabelFromChannel.htm`*

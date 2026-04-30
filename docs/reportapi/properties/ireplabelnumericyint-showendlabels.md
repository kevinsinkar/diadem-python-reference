---
title: "IRepLabelNumericYInt.ShowEndLabels"
description: "Specifies whether DIAdem labels the beginning and the end of the y-axes of a 2D axis system with numbers."
---

# IRepLabelNumericYInt.ShowEndLabels

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShowEndLabels for LabelNumericY

Specifies whether DIAdem labels the beginning and the end of the y-axes of a 2D axis system with numbers.

## Signature

```python
obj.ShowEndLabels
```

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[1]/[1]"
oMyShape.YChannel.Reference = "[1]/[2]"
oMyYNumericLabel = oMy2DAxisSystem.YAxis.Numbers
oMyYNumericLabel.UseCurveColor = True
oMyYNumericLabel.Format = "d.dde"
oMyYNumericLabel.Angle = 0
oMyYNumericLabel.Font.Name = "Tahoma"
oMyYNumericLabel.Font.Size = 3
oMyYNumericLabel.RelativePosition = dd.eRelativePositionLeft
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShowEndLabels_IRepLabelNumericYInt.htm`*

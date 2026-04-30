---
title: "IRepLabelNumericYInt.TextAlignment"
description: "Specifies the alignment of the y-axis scale labels in a 2D axis system in DIAdem REPORT."
---

# IRepLabelNumericYInt.TextAlignment

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: TextAlignment for LabelNumericY

Specifies the alignment of the y-axis scale labels in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.TextAlignment
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eAxisLabelTextAlignmentLeft` | 0 | Left |
| `eAxisLabelTextAlignmentCentric` | 1 | Center |
| `eAxisLabelTextAlignmentRight` | 2 | Right |

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
oMyYNumericLabel.TextAlignment = dd.eAxisLabelTextAlignmentLeft
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_TextAlignment_IRepLabelNumericYInt.htm`*

---
title: "IRepSpiderLabelAdditionalInt.RelativePosition"
description: "Specifies the relative position of a curve to the curve data points in the Line and points display mode in a spider axis system in DIAdem REPORT."
---

# IRepSpiderLabelAdditionalInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for SpiderAdditionalLabel

Specifies the relative position of a curve to the curve data points in the Line and points display mode in a spider axis system in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionPointRightTop` | 0 | Top right |
| `eRelativePositionPointCenter` | 1 | Center |
| `eRelativePositionPointRight` | 2 | Right |
| `eRelativePositionPointRightBottom` | 3 | Bottom right |
| `eRelativePositionPointTop` | 4 | Top |
| `eRelativePositionPointBottom` | 5 | Bottom |
| `eRelativePositionPointLeftTop` | 6 | Top left |
| `eRelativePositionPointLeft` | 7 | Left |
| `eRelativePositionPointLeftBottom` | 8 | Bottom left |
| `eRelativePositionPointCenterClip` | 9 | Centered and clipped |
| `eRelativePositionPointQuadrantRelated` | 10 | Relating to the quadrant |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyAddLabel = oMyCurve.Shape.Extensions.Label
oMyAddLabel.Angle = 0
oMyAddLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyAddLabel.RelativePosition = dd.eRelativePositionPointRight
oMyAddLabel.Font.Bold = True
oMyAddLabel.FromChannel.Visible = True
oMyAddLabel.FromChannel.Channel.Reference = "[5]/[1]"
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.IndexValueVisible = True
oMyAddLabel.IndexValueFormat = "d.d"
oMyAddLabel.TextVisible = True
oMyAddLabel.Text = "MyCurve"
oMyAddLabel.Separator = dd.eLabelSeparatorComma
oMyAddLabel.UseCurveColor = True

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepSpiderLabelAdditionalInt.htm`*

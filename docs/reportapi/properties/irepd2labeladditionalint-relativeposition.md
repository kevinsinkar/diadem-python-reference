---
title: "IRepD2LabelAdditionalInt.RelativePosition"
description: "Specifies the relative position of the curve labels to the curve data points in a 2D axis system in DIAdem REPORT. DIAdem centers the curve end label also for t"
---

# IRepD2LabelAdditionalInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for 2DAdditionalLabel

Specifies the relative position of the curve labels to the curve data points in a 2D axis system in DIAdem REPORT. DIAdem centers the curve end label also for the selection terms eRelativePositionPointCenterClip and eRelativePositionPointQuadrantRelated . For stacked bars the relative position of the curve end label does not refer to the curve data points but to the bar area Above, for example, means the top of the bar and centers the center of the bar.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionPointRightTop` | 0 | Top right |
| `eRelativePositionPointCenter` | 1 | Centered |
| `eRelativePositionPointRight` | 2 | Right |
| `eRelativePositionPointRightBottom` | 3 | Bottom right |
| `eRelativePositionPointTop` | 4 | Top |
| `eRelativePositionPointBottom` | 5 | Bottom |
| `eRelativePositionPointLeftTop` | 6 | Top left |
| `eRelativePositionPointLeft` | 7 | Left |
| `eRelativePositionPointLeftBottom` | 8 | Bottom left |
| `eRelativePositionPointCenterClip` | 9 | Centered and clipped |
| `eRelativePositionPointQuadrantRelated` | 10 | Depends on quadrants |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.Position.Type = dd.e2DLabelPositionAtPoint
oMyLabel.RelativePosition = dd.eRelativePositionPointLeft
oMyLabel.Repetition.Mode = dd.e2DLabelRepetitionMaxNPoints
oMyLabel.Repetition.NValue = 10
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepD2LabelAdditionalInt.htm`*

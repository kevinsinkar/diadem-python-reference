---
title: "IRepPolarLabelAdditionalInt.RelativePosition"
description: "Specifies the relative position of curve label to the curve data points in the Line and points display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarLabelAdditionalInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for PolarAdditionalLabel

Specifies the relative position of curve label to the curve data points in the Line and points display mode in a polar axis system in DIAdem REPORT.

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
| `eRelativePositionPointQuadrantRelated` | 10 | Relating to the quadrant |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyLabel = oMyCurve.Shape.Extensions.Label
oMyLabel.YValueVisible = True
oMyLabel.YValueFormat = "d.dd"
oMyLabel.RelativePosition = dd.eRelativePositionPointCenter
oMyLabel.Repetition.Mode = dd.eLabelRepetitionMaxNPoints
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

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepPolarLabelAdditionalInt.htm`*

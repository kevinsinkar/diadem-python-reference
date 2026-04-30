---
title: "IRepD3LabelAdditionalInt.RelativePosition"
description: "Specifies the relative position of the curve symbols to the curve data points in a 3D axis system in DIAdem REPORT."
---

# IRepD3LabelAdditionalInt.RelativePosition

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RelativePosition for 3DAdditionalLabel

Specifies the relative position of the curve symbols to the curve data points in a 3D axis system in DIAdem REPORT.

## Signature

```python
obj.RelativePosition
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eRelativePositionRightTop` | 0 | Top right |
| `eRelativePositionCenter` | 1 | Centered |
| `eRelativePositionRight` | 2 | Right |
| `eRelativePositionRightBottom` | 3 | Bottom right |
| `eRelativePositionTop` | 4 | Top |
| `eRelativePositionBottom` | 5 | Bottom |
| `eRelativePositionLeftTop` | 6 | Top left |
| `eRelativePositionLeft` | 7 | Left |
| `eRelativePositionLeftBottom` | 8 | Bottom left |
| `eRelativePositionPointCenterClip` | 9 | Centered and clipped |
| `eRelativePositionPointQuadrantRelated` | 10 | Depends on quadrants |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMyShape = oMy3DCurve.Shape
oMyShape.DataStructure = dd.e3DDataStructureTriplet
oMyShape.XChannel.Reference = "[2]/[1]"
oMyShape.YChannel.Reference = "[2]/[2]"
oMyShape.ZChannel.Reference = "[2]/[3]"
oMyLabel = oMyShape.Extensions.Label
oMyLabel.Visible = True
oMyLabel.ZValueVisible = True
oMyLabel.ZValueFormat = "d.ddde"
oMyLabel.Repetition.Mode = dd.e3DLabelRepetitionNthPoint
oMyLabel.Repetition.NValue = 8
oMyLabel.Position.Type = dd.e3DLabelPositionAtPoint
oMyLabel.RelativePosition = dd.eRelativePositionPointBottom
oMyLabel.Font.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RelativePosition_IRepD3LabelAdditionalInt.htm`*

---
title: "IRepAxisMiniTickGridLineInt.LineType"
description: "Specifies the line style of the miniticks in a 2D axis system in DIAdem REPORT."
---

# IRepAxisMiniTickGridLineInt.LineType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineType for AxisMiniTickGridLine

Specifies the line style of the miniticks in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.LineType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineTypeNone` | 0 | None |
| `eLineTypeSolid` | 1 | Line |
| `eLineTypeDashDot` | 2 | Dots and dashes |
| `eLineTypeDashed1` | 3 | Dashes 1 |
| `eLineTypeDashed2` | 4 | Dashes 2 |
| `eLineTypeDotted` | 5 | Dotted |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMySettings = oMy2DAxisSystem.Settings
oMySettings.Grid.DisplayMode = dd.e2DAxisGridModeGrid
oMySettings.Grid.MiniTickGrid.Visible = True
oMyHMiniTick = oMySettings.Grid.MiniTickGrid.LineHorizontal
oMyHMiniTick.Interval = 10
oMyHMiniTick.LineType = dd.eLineTypeDashDot
oMyHMiniTick.Width = dd.eLineWidth0100
oMyVMiniTick = oMySettings.Grid.MiniTickGrid.LineVertical
oMyVMiniTick.Interval = 10
oMyVMiniTick.LineType = dd.eLineTypeDashDot
oMyVMiniTick.Width = dd.eLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LineType_IRepAxisMiniTickGridLineInt.htm`*

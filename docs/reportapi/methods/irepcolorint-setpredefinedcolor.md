---
title: "IRepColorInt.SetPredefinedColor"
description: "Assigns a pre-defined color to an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display the predefined c"
---

# IRepColorInt.SetPredefinedColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetPredefinedColor for Color

Assigns a pre-defined color to an object in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display the predefined colors.

## Signature

```python
obj.SetPredefinedColor(Value)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eColorIndexNone` | 0 | None |
| `eColorIndexBlack` | 1 | Black |
| `eColorIndexRed` | 2 | Red |
| `eColorIndexGreen` | 3 | Green |
| `eColorIndexBlue` | 4 | Blue |
| `eColorIndexViolet` | 5 | Violet |
| `eColorIndexTurquoise` | 6 | Turquoise |
| `eColorIndexGrey` | 7 | Gray |
| `eColorIndexYellow` | 8 | Yellow |
| `eColorIndexDarkRed` | 9 | Dark red |
| `eColorIndexDarkGreen` | 10 | Dark green |
| `eColorIndexDarkBlue` | 11 | Dark blue |
| `eColorIndexDarkViolet` | 12 | Dark violet |
| `eColorIndexDarkTurquoise` | 13 | Dark turquoise |
| `eColorIndexDarkGrey` | 14 | Dark gray |
| `eColorIndexDarkYellow` | 15 | Dark yellow |
| `eColorIndexWhite` | 16 | White |

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem, "My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy2DAxisSystem.Settings.UseIndividualAxisStyle = True
oMyXLine = oMy2DAxisSystem.XAxis.Line
oMyXLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyXLine.UseCurveColor = False
oMyXLine.Width = enumLineWidth0100
oMyYLine = oMy2DAxisSystem.YAxis.Line
oMyYLine.Color.SetPredefinedColor(dd.eColorIndexRed)
oMyYLine.UseCurveColor = False
oMyYLine.Width = enumLineWidth0100
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetPredefinedColor_IRepColorInt.htm`*

---
title: "IRepD2BarFillingInt.Pattern"
description: "Specifies the type of bar filling in a 2D axis system in DIAdem REPORT."
---

# IRepD2BarFillingInt.Pattern

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Pattern for 2DBarFilling

Specifies the type of bar filling in a 2D axis system in DIAdem REPORT.

## Signature

```python
obj.Pattern
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eFillPatternNone` | 0 | None |
| `eFillPatternRightDiagonal` | 1 | Right diagonal |
| `eFillPatternLeftDiagonal` | 2 | Left diagonal |
| `eFillPatternCrossDiagonal` | 3 | Cross diagonal |
| `eFillPatternHorizontal` | 4 | Horizontal |
| `eFillPatternVertical` | 5 | Vertical |
| `eFillPatternGrid` | 6 | Grid |
| `eFillPatternFilled` | 7 | Filled |

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
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeBars, "MyCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference = "[6]/[1]"
oMyShape.YChannel.Reference = "[6]/[2]"
oMySettings = oMyShape.Settings
oMySettings.BorderLine.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyFilling = oMySettings.Filling
oMyFilling.UseSameColorAsBorder = False
oMyFilling.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyFilling.Pattern = dd.eFillPatternCrossDiagonal
oMyFilling.Density = 30
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Pattern_IRepD2BarFillingInt.htm`*

---
title: "IRepBoxWhiskerMarkerFillingInt.SetPredefinedColor"
description: "Uses the display mode Box whisker to assign a predefined color to a marker filling in a 2D axis system in DIAdem REPORT. The method also specifies the Color obj"
---

# IRepBoxWhiskerMarkerFillingInt.SetPredefinedColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetPredefinedColor for 2DBoxWhiskerMarkerFilling

Uses the display mode Box whisker to assign a predefined color to a marker filling in a 2D axis system in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display the predefined colors.

## Signature

```python
obj.SetPredefinedColor(Value)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePredefinedColorNone` | 0 | None |
| `ePredefinedColorBlack` | 1 | Black |
| `ePredefinedColorRed` | 2 | Red |
| `ePredefinedColorGreen` | 3 | Green |
| `ePredefinedColorBlue` | 4 | Blue |
| `ePredefinedColorViolet` | 5 | Violet |
| `ePredefinedColorTurquoise` | 6 | Turquoise |
| `ePredefinedColorGrey` | 7 | Gray |
| `ePredefinedColorYellow` | 8 | Yellow |
| `ePredefinedColorDarkRed` | 9 | Dark red |
| `ePredefinedColorDarkGreen` | 10 | Dark green |
| `ePredefinedColorDarkBlue` | 11 | Dark blue |
| `ePredefinedColorDarkViolet` | 12 | Dark violet |
| `ePredefinedColorDarkTurquoise` | 13 | Dark turquoise |
| `ePredefinedColorDarkGrey` | 14 | Dark gray |
| `ePredefinedColorDarkYellow` | 15 | Dark yellow |
| `ePredefinedColorWhite` | 16 | White |

## Python example

```python
o2DCurve = dd.Report.ActiveSheet.Objects.Item("").Curves2D.Item("2DAxis2_Curve1")
o2DBoxWhisker = o2DCurve.Shape
o2DBoxWhisker.Extensions.MarkerBox.Filling.SetPredefinedColor(dd.ePredefinedColorDarkRed)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetPredefinedColor_IRepBoxWhiskerMarkerFillingInt.htm`*

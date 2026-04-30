---
title: "IRepBoxWhiskerMarkerFillingInt.ColorIndex"
description: "Specifies the color of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT. DIAdem only includes the ColorIndex proper"
---

# IRepBoxWhiskerMarkerFillingInt.ColorIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColorIndex for 2DBoxWhiskerMarkerFilling

Specifies the color of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT. DIAdem only includes the ColorIndex property if you assign the value FALSE to the UseBorderColor property. DIAdem does not support the value eColorIndexFillEffects for markers.

## Signature

```python
obj.ColorIndex
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
| `eColorIndexOtherColors` | 17 | Other colors |
| `eColorIndexPalette` | 18 | Palette |
| `eColorIndexGlobalColorPalette1` | 19 | Global palette 1 |
| `eColorIndexGlobalColorPalette2` | 20 | Global palette 2 |
| `eColorIndexGlobalColorPalette3` | 21 | Global palette 3 |
| `eColorIndexFillEffects` | 22 | Filling effects |

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerWhisker.Filling.UseBorderColor = False
o2DBoxWhisker.Extensions.MarkerWhisker.Filling.ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColorIndex_IRepBoxWhiskerMarkerFillingInt.htm`*

---
title: "IRepBackgroundColorInt.ColorIndex"
description: "Specifies the highlighting color of an object in DIAdem REPORT."
---

# IRepBackgroundColorInt.ColorIndex

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ColorIndex for BackgroundColor

Specifies the highlighting color of an object in DIAdem REPORT.

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
oAxisLabel = dd.Report.ActiveSheet.Objects.Item("2DAxis1").XAxis.Label
oAxisLabel.Font.BackColor.ColorIndex = dd.eColorIndexRed
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ColorIndex_IRepBackgroundColorInt.htm`*

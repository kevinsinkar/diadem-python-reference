---
title: "IRepBoxWhiskerMarkerInt.Type"
description: "Specifies in a 2D axis system in the Box Whisker display mode in DIAdem-REPORT the symbol with which DIAdem displays outliers, values within the whisker, and va"
---

# IRepBoxWhiskerMarkerInt.Type

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Type for 2DBoxWhiskerMarker

Specifies in a 2D axis system in the Box Whisker display mode in DIAdem-REPORT the symbol with which DIAdem displays outliers, values within the whisker, and values within the box.

## Signature

```python
obj.Type
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eMarkerNone` | 0 | None |
| `eMarkerSquare` | 1 | Square |
| `eMarkerRhombus` | 2 | Rhombus |
| `eMarkerTriangle` | 3 | Triangle |
| `eMarkerCross` | 4 | Cross |
| `eMarkerAsterisk` | 5 | Asterisk |
| `eMarkerShortDash` | 6 | Short dash |
| `eMarkerLongDash` | 7 | Long dash |
| `eMarkerPlus` | 8 | Plus |
| `eMarkerCircle` | 9 | Circle |
| `eMarkerTriangle_Bottom` | 10 | Triangle bottom |
| `eMarkerTriangle_Left` | 11 | Triangle left |
| `eMarkerTriangle_Right` | 12 | Triangle right |
| `eMarkerSquare_Top` | 13 | Square filled top |
| `eMarkerSquare_Bottom` | 14 | Square filled bottom |
| `eMarkerSquare_Left` | 15 | Square filled left |
| `eMarkerSquare_Right` | 16 | Square filled right |
| `eMarkerRhomb_Top` | 17 | Rhombus filled top |
| `eMarkerRhomb_Bottom` | 18 | Rhombus filled bottom |
| `eMarkerRhomb_Left` | 19 | Rhombus filled left |
| `eMarkerRhomb_Right` | 20 | Rhombus filled right |
| `eMarkerTriangle1_Left` | 21 | Triangle 1 filled left |
| `eMarkerTriangle1_Right` | 22 | Triangle 1 filled right |
| `eMarkerTriangle2_Left` | 23 | Triangle 2 filled left |
| `eMarkerTriangle2_Right` | 24 | Triangle 2 filled right |
| `eMarkerTriangle3_Top` | 25 | Triangle 3 filled top |
| `eMarkerTriangle3_Bottom` | 26 | Triangle 3 filled bottom |
| `eMarkerTriangle4_Top` | 27 | Triangle 4 filled top |
| `eMarkerTriangle4_Bottom` | 28 | Triangle 4 filled bottom |

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerWhisker.Type = dd.eMarkerCircle
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Type_IRepBoxWhiskerMarkerInt.htm`*

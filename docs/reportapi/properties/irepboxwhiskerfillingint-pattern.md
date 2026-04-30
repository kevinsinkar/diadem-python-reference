---
title: "IRepBoxWhiskerFillingInt.Pattern"
description: "Specifies the filling type of the box in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerFillingInt.Pattern

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Pattern for 2DBoxWhiskerFilling

Specifies the filling type of the box in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

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
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.Filling.LineWidth = dd.eLineWidth0070
o2DBoxWhisker.Settings.Filling.Pattern = dd.eFillPatternLeftDiagonal
o2DBoxWhisker.Settings.Filling.Density = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Pattern_IRepBoxWhiskerFillingInt.htm`*

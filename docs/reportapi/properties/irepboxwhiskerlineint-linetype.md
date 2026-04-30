---
title: "IRepBoxWhiskerLineInt.LineType"
description: "Specifies the line style in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerLineInt.LineType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: LineType for 2DBoxWhiskerLine

Specifies the line style in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

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
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.WhiskerLine.LineType = dd.eLineTypeDashDot
o2DBoxWhisker.Settings.WhiskerLine.Interval = 1
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_LineType_IRepBoxWhiskerLineInt.htm`*

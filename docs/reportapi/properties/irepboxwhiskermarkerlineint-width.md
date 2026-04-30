---
title: "IRepBoxWhiskerMarkerLineInt.Width"
description: "Specifies the line width of the additional markers in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerMarkerLineInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for 2DBoxWhiskerMarkerLine

Specifies the line width of the additional markers in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
obj.Width
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eLineWidthMin` | 0 | Minimum |
| `eLineWidth0025` | 1 | 0.25 |
| `eLineWidth0035` | 2 | 0.35 |
| `eLineWidth0050` | 3 | 0.5 |
| `eLineWidth0070` | 4 | 0.7 |
| `eLineWidth0100` | 5 | 1.0 |
| `eLineWidth0140` | 6 | 1.4 |
| `eLineWidth0200` | 7 | 2.0 |
| `eLineWidth0280` | 8 | 2.8 |
| `eLineWidth0400` | 9 | 4.0 |
| `eLineWidth0560` | 10 | 5.6 |
| `eLineWidth0800` | 11 | 8.0 |
| `eLineWidth1120` | 12 | 11.2 |
| `eLineWidth1600` | 13 | 16.0 |
| `eLineWidth2240` | 14 | 22.4 |
| `eLineWidth3200` | 15 | 32.0 |

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerWhisker.Line.Width = dd.eLineWidth0050
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepBoxWhiskerMarkerLineInt.htm`*

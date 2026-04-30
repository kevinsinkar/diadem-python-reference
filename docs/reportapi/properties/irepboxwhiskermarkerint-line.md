---
title: "IRepBoxWhiskerMarkerInt.Line"
description: "Specifies the line property of the additional markers in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerMarkerInt.Line

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Line for 2DBoxWhiskerMarker

Specifies the line property of the additional markers in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Line
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerWhisker.Line.UseBorderColor = False
o2DBoxWhisker.Extensions.MarkerWhisker.Line.Color.ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Line_IRepBoxWhiskerMarkerInt.htm`*

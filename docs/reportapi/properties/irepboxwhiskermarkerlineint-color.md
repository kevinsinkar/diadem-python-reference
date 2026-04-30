---
title: "IRepBoxWhiskerMarkerLineInt.Color"
description: "Specifies the line color of the additional markers in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerMarkerLineInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for 2DBoxWhiskerMarkerLine

Specifies the line color of the additional markers in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
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

*Source: `ReportApi/properties/Report_property_Color_IRepBoxWhiskerMarkerLineInt.htm`*

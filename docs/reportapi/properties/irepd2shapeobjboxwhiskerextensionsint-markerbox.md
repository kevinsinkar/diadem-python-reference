---
title: "IRepD2ShapeObjBoxWhiskerExtensionsInt.MarkerBox"
description: "Specifies the properties of the additional markers within a box in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerExtensionsInt.MarkerBox

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: MarkerBox for 2DBoxWhiskerExtensions

Specifies the properties of the additional markers within a box in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.MarkerBox
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerBox.Line.Width = dd.eLineWidth0070
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_MarkerBox_IRepD2ShapeObjBoxWhiskerExtensionsInt.htm`*

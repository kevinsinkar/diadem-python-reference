---
title: "IRepD2ShapeObjBoxWhiskerInt.Extensions"
description: "Specifies the extended properties of a curve in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerInt.Extensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Extensions for 2DBoxWhisker

Specifies the extended properties of a curve in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Extensions
```

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

*Source: `ReportApi/properties/Report_property_Extensions_IRepD2ShapeObjBoxWhiskerInt.htm`*

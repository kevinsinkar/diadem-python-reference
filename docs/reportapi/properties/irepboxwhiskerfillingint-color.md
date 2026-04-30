---
title: "IRepBoxWhiskerFillingInt.Color"
description: "Specifies the filling color of a Box Whisker plot in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerFillingInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for 2DBoxWhiskerFilling

Specifies the filling color of a Box Whisker plot in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.Filling.Color.ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepBoxWhiskerFillingInt.htm`*

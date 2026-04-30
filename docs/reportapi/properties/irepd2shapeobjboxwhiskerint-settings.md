---
title: "IRepD2ShapeObjBoxWhiskerInt.Settings"
description: "Specifies the properties of a bar in the Box Whisker display mode in a 2D axis system in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DBoxWhisker

Specifies the properties of a bar in the Box Whisker display mode in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
o2DCurve = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1")
o2DBoxWhisker = o2DCurve.Shape
o2DBoxWhisker.Settings.BorderLine.Color.ColorIndex = dd.eColorIndexDarkRed
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepD2ShapeObjBoxWhiskerInt.htm`*

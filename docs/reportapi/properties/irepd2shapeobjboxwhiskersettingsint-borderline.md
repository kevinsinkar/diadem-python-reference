---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt.BorderLine"
description: "Specifies the frame line of a Box Whisker plot in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerSettingsInt.BorderLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: BorderLine for 2DBoxWhiskerSettings

Specifies the frame line of a Box Whisker plot in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.BorderLine
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

*Source: `ReportApi/properties/Report_property_BorderLine_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*

---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt.Filling"
description: "Specifies the properties of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepD2ShapeObjBoxWhiskerSettingsInt.Filling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Filling for 2DBoxWhiskerSettings

Specifies the properties of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Filling
```

## Python example

```python
o2DCurve = dd.Report.ActiveSheet.Objects.Item("").Curves2D.Item("2DAxis2_Curve1")
o2DBoxWhisker = o2DCurve.Shape
o2DBoxWhisker.Extensions.MarkerBox.Filling.SetPredefinedColor(dd.ePredefinedColorDarkRed)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Filling_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*

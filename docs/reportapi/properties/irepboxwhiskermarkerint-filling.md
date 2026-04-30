---
title: "IRepBoxWhiskerMarkerInt.Filling"
description: "Specifies the properties of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerMarkerInt.Filling

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Filling for 2DBoxWhiskerMarker

Specifies the properties of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
return_value = obj.Filling
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.Filling.Color.ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Filling_IRepBoxWhiskerMarkerInt.htm`*

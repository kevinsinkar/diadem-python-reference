---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt.Width"
description: "Specifies the box width in a 2D axis system in the Box-Whisker display mode in DIAdem REPORT. The percentage refers to the available whisker width. At 20 displa"
---

# IRepD2ShapeObjBoxWhiskerSettingsInt.Width

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Width for 2DBoxWhiskerSettings

Specifies the box width in a 2D axis system in the Box-Whisker display mode in DIAdem REPORT. The percentage refers to the available whisker width. At 20 displayed points, 100% corresponds to one twentieth of the width of the axis system.

## Signature

```python
obj.Width
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.Width = 30
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Width_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*

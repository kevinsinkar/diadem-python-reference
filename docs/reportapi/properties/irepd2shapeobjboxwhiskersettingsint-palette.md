---
title: "IRepD2ShapeObjBoxWhiskerSettingsInt.Palette"
description: "Specifies the properties of the palette DIAdem REPORT uses in a 2D axis system in the Box Whisker display mode."
---

# IRepD2ShapeObjBoxWhiskerSettingsInt.Palette

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Palette for 2DBoxWhiskerSettings

Specifies the properties of the palette DIAdem REPORT uses in a 2D axis system in the Box Whisker display mode.

## Signature

```python
return_value = obj.Palette
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.Palette.Colors.Item(1).ColorIndex = dd.eColorIndexBlue
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Palette_IRepD2ShapeObjBoxWhiskerSettingsInt.htm`*

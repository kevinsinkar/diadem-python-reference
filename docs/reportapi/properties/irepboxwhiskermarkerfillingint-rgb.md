---
title: "IRepBoxWhiskerMarkerFillingInt.RGB"
description: "Specifies the RGB values of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT. First assign the value eColorIndexOth"
---

# IRepBoxWhiskerMarkerFillingInt.RGB

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: RGB for 2DBoxWhiskerMarkerFilling

Specifies the RGB values of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT. First assign the value eColorIndexOtherColors to the property ColorIndex . You also can use the SetRGBColor method to specify individual colors. Use the SetFillingColor method to specify filling effects.

## Signature

```python
obj.RGB
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis2").Curves2D.Item("2DAxis2_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerBox.Filling.ColorIndex = dd.eColorIndexFillEffects
o2DBoxWhisker.Extensions.MarkerBox.Filling.UseBorderColor = False
o2DBoxWhisker.Extensions.MarkerBox.Filling.RGB = dd.RGB(255, 0, 0)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_RGB_IRepBoxWhiskerMarkerFillingInt.htm`*

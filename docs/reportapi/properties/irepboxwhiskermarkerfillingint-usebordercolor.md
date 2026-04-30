---
title: "IRepBoxWhiskerMarkerFillingInt.UseBorderColor"
description: "Specifies whether DIAdem-REPORT also uses the line color of the box for the filling of additional markers in a 2D axis system in the Box Whisker display mode."
---

# IRepBoxWhiskerMarkerFillingInt.UseBorderColor

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: UseBorderColor for 2DBoxWhiskerMarkerFilling

Specifies whether DIAdem-REPORT also uses the line color of the box for the filling of additional markers in a 2D axis system in the Box Whisker display mode.

## Signature

```python
obj.UseBorderColor
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

*Source: `ReportApi/properties/Report_property_UseBorderColor_IRepBoxWhiskerMarkerFillingInt.htm`*

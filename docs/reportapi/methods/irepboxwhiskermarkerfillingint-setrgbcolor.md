---
title: "IRepBoxWhiskerMarkerFillingInt.SetRGBColor"
description: "Assigns a color to a marker of a box whisker display in a 2D axis system in DIAdem REPORT. The method also specifies the Color object properties which are neces"
---

# IRepBoxWhiskerMarkerFillingInt.SetRGBColor

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: SetRGBColor for 2DBoxWhiskerMarkerFilling

Assigns a color to a marker of a box whisker display in a 2D axis system in DIAdem REPORT. The method also specifies the Color object properties which are necessary to display a color.

## Signature

```python
obj.SetRGBColor(RGB)
```

## Python example

```python
o2DCurve = dd.Report.ActiveSheet.Objects.Item("2DAxis2").Curves2D.Item("2DAxis2_Curve1")
o2DBoxWhisker = o2DCurve.Shape
o2DBoxWhisker.Extensions.MarkerBox.Filling.SetRGBColor(dd.RGB(255,0,0))
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_SetRGBColor_IRepBoxWhiskerMarkerFillingInt.htm`*

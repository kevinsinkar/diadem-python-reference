---
title: "IRepBoxWhiskerMarkerFillingInt.Transparency"
description: "Specifies the transpancy percent of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT. The value 100 specifies a com"
---

# IRepBoxWhiskerMarkerFillingInt.Transparency

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Transparency for 2DBoxWhiskerMarkerFilling

Specifies the transpancy percent of the curve marker filling of a 2D axis system in the Box Whisker display mode in DIAdem REPORT. The value 100 specifies a completely transparent display and the value 0 specifies a completely opaque display. Not all DIAdem objects display transparency.

## Signature

```python
obj.Transparency
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis2").Curves2D.Item("2DAxis2_Curve1").Shape
o2DBoxWhisker.Extensions.MarkerWhisker.Filling.UseBorderColor = False
o2DBoxWhisker.Extensions.MarkerWhisker.Filling.ColorIndex = dd.eColorIndexBlue
o2DBoxWhisker.Extensions.MarkerWhisker.Filling.Transparency = 50
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Transparency_IRepBoxWhiskerMarkerFillingInt.htm`*

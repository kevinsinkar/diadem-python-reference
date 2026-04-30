---
title: "IRepBoxWhiskerFillingInt.Density"
description: "Specifies the hatching density of the box filling in a 2D axis system in the Box Whisker display mode in DIAdem REPORT."
---

# IRepBoxWhiskerFillingInt.Density

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Density for 2DBoxWhiskerFilling

Specifies the hatching density of the box filling in a 2D axis system in the Box Whisker display mode in DIAdem REPORT.

## Signature

```python
obj.Density
```

## Python example

```python
o2DBoxWhisker = dd.Report.ActiveSheet.Objects.Item("2DAxis1").Curves2D.Item("2DAxis1_Curve1").Shape
o2DBoxWhisker.Settings.Filling.LineWidth = dd.eLineWidth0070
o2DBoxWhisker.Settings.Filling.Pattern = dd.eFillPatternLeftDiagonal
o2DBoxWhisker.Settings.Filling.Density = 20
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Density_IRepBoxWhiskerFillingInt.htm`*

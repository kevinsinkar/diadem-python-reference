---
title: "IRepLineFullFeaturedInt.Color"
description: "Specifies the line color of a curve in DIAdem REPORT."
---

# IRepLineFullFeaturedInt.Color

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Color for FullFeaturedLine

Specifies the line color of a curve in DIAdem REPORT.

## Signature

```python
return_value = obj.Color
```

## Python example

```python
dd.Report.NewLayout()
oMy2DaxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMy2DCurve = oMy2DaxisSystem.Curves2D.Add(dd.e2DShapeLine, "MyNew2DCurve")
oMy2DCurve.Shape.XChannel.Reference = "[1]/[1]"
oMy2DCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DCurve.Shape.Settings.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Color_IRepLineFullFeaturedInt.htm`*

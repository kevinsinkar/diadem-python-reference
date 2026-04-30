---
title: "IRepD2AxisInt.Settings"
description: "Specifies the general settings of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisInt.Settings

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Settings for 2DAxisSystem

Specifies the general settings of a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Settings
```

## Python example

```python
dd.Report.NewLayout()
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.Settings.BackgroundColor.SetPredefinedColor(dd.eColorIndexYellow)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Settings_IRepD2AxisInt.htm`*

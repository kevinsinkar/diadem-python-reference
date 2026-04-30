---
title: "IRepD2AxisInt.YAxis"
description: "Specifies the properties of the first y-axis in a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisInt.YAxis

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YAxis for 2DAxisSystem

Specifies the properties of the first y-axis in a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.YAxis
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Example.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.XAxis.TargetUnit = "h"
oMy2DAxisSystem.YAxis.TargetUnit = "km/h"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso">
<h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YAxis_IRepD2AxisInt.htm`*

---
title: "IRepD2AxisInt.Curves2D"
description: "Returns a collection of all curves in a 2D axis system of DIAdem REPORT."
---

# IRepD2AxisInt.Curves2D

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Curves2D for 2DAxisSystem

Returns a collection of all curves in a 2D axis system of DIAdem REPORT.

## Signature

```python
return_value = obj.Curves2D
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPos = oMy2DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMy2DAxisSystem.Curves2D.Add(dd.e2DShapeLine,"My2DCurve")
oMyCurve.Shape.XChannel.Reference = "[1]/[1]"
oMyCurve.Shape.YChannel.Reference = "[1]/[2]"
oMy2DAxisSystem.CurveLegend.Visible = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Curves2D_IRepD2AxisInt.htm`*

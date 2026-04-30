---
title: "IRepD2AxisInt.CurveLegend"
description: "Specifies the curve legend of a 2D axis system in DIAdem REPORT."
---

# IRepD2AxisInt.CurveLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CurveLegend for 2DAxisSystem

Specifies the curve legend of a 2D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.CurveLegend
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy2DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject2DAxisSystem,"My2DAxisSystem")
oMyPosition = oMy2DAxisSystem.Position.ByBorder
oMyPosition.Top = 30
oMyPosition.Bottom = 20
oMyPosition.Left = 20
oMyPosition.Right = 30
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

*Source: `ReportApi/properties/Report_property_CurveLegend_IRepD2AxisInt.htm`*

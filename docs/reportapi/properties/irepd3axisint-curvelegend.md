---
title: "IRepD3AxisInt.CurveLegend"
description: "Specifies the curve legend of a 3D axis system in DIAdem REPORT."
---

# IRepD3AxisInt.CurveLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CurveLegend for 3DAxisSystem

Specifies the curve legend of a 3D axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.CurveLegend
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMy3DAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObject3DAxisSystem,"My3DAxisSystem")
oMyPos = oMy3DAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMy3DCurve = oMy3DAxisSystem.Curves3D.Add(dd.e3DShapeSurface, "MyNew3DCurve")
oMy3DCurve.Shape.XChannel.Reference = "[2]/[1]"
oMy3DCurve.Shape.YChannel.Reference = "[2]/[2]"
oMy3DCurve.Shape.ZChannel.Reference = "[2]/[3]"
oMy3DCurve.Shape.DataStructure = dd.e3DDataStructureMatrix
oMyCurveLegend = oMy3DAxisSystem.CurveLegend
oMyCurveLegend.Visible = True
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CurveLegend_IRepD3AxisInt.htm`*

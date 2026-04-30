---
title: "IRepPolarShapeObjDifferentialInt.DifferentialLine"
description: "Specifies the curve properties in the Differential display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjDifferentialInt.DifferentialLine

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DifferentialLine for PolarDifferential

Specifies the curve properties in the Differential display mode in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.DifferentialLine
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPolarAxisSystem.Position.ByCoordinate.X1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.Y1 = 20
oMyPolarAxisSystem.Position.ByCoordinate.X2 = 80
oMyPolarAxisSystem.Position.ByCoordinate.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeDifferential, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.YChannelDifferential.Reference = "[5]/[3]"
oMyCurve.Shape.DifferentialLine.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
oMyCurve.Shape.DifferentialLine.LineType = dd.eLineTypeDashed1
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DifferentialLine_IRepPolarShapeObjDifferentialInt.htm`*

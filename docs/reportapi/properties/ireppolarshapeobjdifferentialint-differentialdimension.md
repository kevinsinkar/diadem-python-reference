---
title: "IRepPolarShapeObjDifferentialInt.DifferentialDimension"
description: "Specifies the width and the displacement of a curve in the Differential display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjDifferentialInt.DifferentialDimension

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: DifferentialDimension for PolarDifferential

Specifies the width and the displacement of a curve in the Differential display mode in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.DifferentialDimension
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyPosition = oMyPolarAxisSystem.Position.ByCoordinate
oMyPosition.X1 = 20
oMyPosition.Y1 = 20
oMyPosition.X2 = 80
oMyPosition.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeDifferential, "MyNewCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference= "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMyShape.YChannelDifferential.Reference = "[5]/[3]"
oMyShape.DifferentialDimension.Offset = 10
oMyShape.DifferentialDimension.Width = 20
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_DifferentialDimension_IRepPolarShapeObjDifferentialInt.htm`*

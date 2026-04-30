---
title: "IRepPolarShapeObjDifferentialInt.YChannel"
description: "Specifies the first y-channel of a curve in the Differential display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjDifferentialInt.YChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannel for PolarDifferential

Specifies the first y-channel of a curve in the Differential display mode in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.YChannel
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
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.YChannelDifferential.Reference = "[5]/[3]"
oMyCurve.Shape.DifferentialLine.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannel_IRepPolarShapeObjDifferentialInt.htm`*

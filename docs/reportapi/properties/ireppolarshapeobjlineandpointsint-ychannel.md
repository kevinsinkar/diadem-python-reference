---
title: "IRepPolarShapeObjLineAndPointsInt.YChannel"
description: "Specifies the y-channel of a curve in the Line and points display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjLineAndPointsInt.YChannel

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: YChannel for PolarLineAndPoints

Specifies the y-channel of a curve in the Line and points display mode in a polar axis system in DIAdem REPORT.

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
oMyShape = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyNewCurve").Shape
oMyShape.XChannel.Reference = "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMyShape.Extensions.Label.Repetition.Mode = dd.eLabelRepetitionNthPoint
oMyShape.Points.XValueVisible = True
oMyShape.Points.DisplayEveryNthPoint = 200
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_YChannel_IRepPolarShapeObjLineAndPointsInt.htm`*

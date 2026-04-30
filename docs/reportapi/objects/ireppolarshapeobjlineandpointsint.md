---
title: "IRepPolarShapeObjLineAndPointsInt"
description: "The PolarLineAndPoints object provides the properties of a curve in the Line and points display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjLineAndPointsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarLineAndPoints

The PolarLineAndPoints object provides the properties of a curve in the Line and points display mode in a polar axis system in DIAdem REPORT.

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
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLineAndPoints, "MyNewCurve")
oMyShape = oMyCurve.Shape
oMyShape.XChannel.Reference= "[5]/[1]"
oMyShape.YChannel.Reference = "[5]/[2]"
oMyShape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
oMyShape.Extensions.Label.Repetition.Mode = dd.eLabelRepetitionNthPoint
oMyPoints = oMyShape.Settings.Points
oMyPoints.YValueFormat = "d.d"
oMyPoints.YValueVisible = True
oMyPoints.DisplayEveryNthPoint = 50
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarshapeobjlineandpointsint-extensions/">Extensions</a> | <a href="../../properties/ireppolarshapeobjlineandpointsint-settings/">Settings</a> | <a href="../../properties/ireppolarshapeobjlineandpointsint-xchannel/">XChannel</a> | <a href="../../properties/ireppolarshapeobjlineandpointsint-ychannel/">YChannel</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarcurveint/">PolarCurve</a>.<a href="../../properties/ireppolarcurveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarShapeObjLineAndPointsInt.htm`*

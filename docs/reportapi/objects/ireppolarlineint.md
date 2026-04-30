---
title: "IRepPolarLineInt"
description: "The PolarCurveLine object provides the curve properties in the Line display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarLineInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarCurveLine

The PolarCurveLine object provides the curve properties in the Line display mode in a polar axis system in DIAdem REPORT.

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
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Width = dd.eLineWidth0070
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexDarkRed)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarlineint-color/">Color</a> | <a href="../../properties/ireppolarlineint-connectnovalueneighbors/">ConnectNoValueNeighbors</a> | <a href="../../properties/ireppolarlineint-interval/">Interval</a> | <a href="../../properties/ireppolarlineint-linetype/">LineType</a> | <a href="../../properties/ireppolarlineint-width/">Width</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../ireppolarshapeobjlineint/">PolarLine</a>.<a href="../../properties/ireppolarshapeobjlineint-line/">Line</a> | <a href="../ireppolarshapeobjlineandpointssettingsint/">PolarLineAndPointsSettings</a>.<a href="../../properties/ireppolarshapeobjlineandpointssettingsint-line/">Line</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepPolarLineInt.htm`*

---
title: "IRepPolarShapeObjBaseInt"
description: "The PolarShapeObject object provides the properties of a curve in a polar axis system in DIAdem REPORT. The PolarShapeObject object corresponds to one of the fo"
---

# IRepPolarShapeObjBaseInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarShapeObject

The PolarShapeObject object provides the properties of a curve in a polar axis system in DIAdem REPORT. The PolarShapeObject object corresponds to one of the following objects: PolarDifferential (IRepPolarShapeObjDifferentialInt) Differential PolarLine (IRepPolarShapeObjLineInt) Line PolarLineAndPoints (IRepPolarShapeObjLineAndPointsInt) Line and points PolarSpike (IRepPolarShapeObjSpikesInt) Spikes

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
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarshapeobjbaseint-xchannel/">XChannel</a> | <a href="../../properties/ireppolarshapeobjbaseint-ychannel/">YChannel</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepPolarShapeObjBaseInt.htm`*

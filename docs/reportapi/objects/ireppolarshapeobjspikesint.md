---
title: "IRepPolarShapeObjSpikesInt"
description: "The PolarSpike object provides the curve properties in the Spikes display mode in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjSpikesInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: PolarSpike

The PolarSpike object provides the curve properties in the Spikes display mode in a polar axis system in DIAdem REPORT.

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
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeSpikes, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Spike.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/ireppolarshapeobjspikesint-spike/">Spike</a> | <a href="../../properties/ireppolarshapeobjspikesint-xchannel/">XChannel</a> | <a href="../../properties/ireppolarshapeobjspikesint-ychannel/">YChannel</a></p>
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

*Source: `ReportApi/Objects/Report_Objects_IRepPolarShapeObjSpikesInt.htm`*

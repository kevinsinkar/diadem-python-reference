---
title: "IRepPolarShapeObjSpikesInt.Spike"
description: "Specifies the properties of a spike display in a polar axis system in DIAdem REPORT."
---

# IRepPolarShapeObjSpikesInt.Spike

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Spike for PolarSpike

Specifies the properties of a spike display in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Spike
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
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeSpikes, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Spike.Color.SetPredefinedColor(dd.eColorIndexDarkBlue)
oMyCurve.Shape.Spike.LineType = dd.eLineTypeSolid
oMyCurve.Shape.Spike.Width = dd.eLineWidth0025
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Spike_IRepPolarShapeObjSpikesInt.htm`*

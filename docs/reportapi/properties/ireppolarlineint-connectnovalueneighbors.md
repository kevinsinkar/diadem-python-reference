---
title: "IRepPolarLineInt.ConnectNoValueNeighbors"
description: "Specifies whether DIAdem REPORT connects NoValues with the neighboring curve points in a polar axis system."
---

# IRepPolarLineInt.ConnectNoValueNeighbors

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ConnectNoValueNeighbors for PolarCurveLine

Specifies whether DIAdem REPORT connects NoValues with the neighboring curve points in a polar axis system.

## Signature

```python
obj.ConnectNoValueNeighbors
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.ConnectNoValueNeighbors = True
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ConnectNoValueNeighbors_IRepPolarLineInt.htm`*

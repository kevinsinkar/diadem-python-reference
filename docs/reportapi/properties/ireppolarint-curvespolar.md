---
title: "IRepPolarInt.CurvesPolar"
description: "Returns a collection of all curves in a polar axis system in DIAdem REPORT."
---

# IRepPolarInt.CurvesPolar

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: CurvesPolar for PolarSystem

Returns a collection of all curves in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.CurvesPolar
```

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
oMyPolarAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarAxisSystem")
oMyPos = oMyPolarAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyCurve")
oMyCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_CurvesPolar_IRepPolarInt.htm`*

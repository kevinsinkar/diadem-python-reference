---
title: "IRepPolarCurveInt.Shape"
description: "Specifies the design of a polar curve in DIAdem REPORT."
---

# IRepPolarCurveInt.Shape

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Shape for PolarCurve

Specifies the design of a polar curve in DIAdem REPORT.

## Signature

```python
return_value = obj.Shape
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarSystem")
oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyPolarCurve.Shape.YChannel.Reference = "[5]/[2]"
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Shape_IRepPolarCurveInt.htm`*

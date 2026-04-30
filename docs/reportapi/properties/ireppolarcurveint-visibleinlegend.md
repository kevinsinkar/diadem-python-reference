---
title: "IRepPolarCurveInt.VisibleInLegend"
description: "Specifies whether DIAdem REPORT displays the legend item that belongs to a curve in a polar axis system."
---

# IRepPolarCurveInt.VisibleInLegend

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: VisibleInLegend for PolarCurve

Specifies whether DIAdem REPORT displays the legend item that belongs to a curve in a polar axis system.

## Signature

```python
obj.VisibleInLegend
```

## Python example

```python
dd.Report.NewLayout()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem, "MyPolarSystem")
oMyPos = oMyPolarSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80
oMyPolarCurve = oMyPolarSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyPolarCurve")
oMyPolarCurve.Shape.XChannel.Reference = "[5]/[1]"
oMyPolarCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyPolarSystem.CurveLegend.Visible = True
oMyPolarCurve.VisibleInLegend = False
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_VisibleInLegend_IRepPolarCurveInt.htm`*

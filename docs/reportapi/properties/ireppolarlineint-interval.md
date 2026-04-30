---
title: "IRepPolarLineInt.Interval"
description: "Specifies the line interval for broken lines in a polar axis system in DIAdem REPORT. Greater values mean greater intervals."
---

# IRepPolarLineInt.Interval

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Interval for PolarCurveLine

Specifies the line interval for broken lines in a polar axis system in DIAdem REPORT. Greater values mean greater intervals.

## Signature

```python
obj.Interval
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
OMyCurve = oMyPolarAxisSystem.CurvesPolar.Add(dd.ePolarShapeLine, "MyCurve")
OMyCurve.Shape.XChannel.Reference = "[5]/[1]"
OMyCurve.Shape.YChannel.Reference = "[5]/[2]"
OMyCurve.Shape.Line.LineType = dd.eLineTypeDashed1
OMyCurve.Shape.Line.Interval = 5
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Interval_IRepPolarLineInt.htm`*

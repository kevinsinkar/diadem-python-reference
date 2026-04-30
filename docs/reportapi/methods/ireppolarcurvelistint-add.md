---
title: "IRepPolarCurveListInt.Add"
description: "Generates a new curve in a polar axis system in DIAdem REPORT."
---

# IRepPolarCurveListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for PolarCurves

Generates a new curve in a polar axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(ShapeType, Name)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `ePolarShapeLine` | 0 | Line |
| `ePolarShapeLineAndPoints` | 1 | Line and points |
| `ePolarShapeSpikes` | 2 | Spikes |
| `ePolarShapeDifferential` | 3 | Differential |

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad(dd.DataReadPath + "Report_Data.tdm","TDM","")
dd.Report.NewLayout()
oMyPolarAxisSys = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectPolarSystem,"MyPolarSystem")
oMyCurve = oMyPolarAxisSys.CurvesPolar.Add(dd.ePolarShapeLine, "MyNewCurve")
oMyCurve.Shape.XChannel.Reference= "[5]/[1]"
oMyCurve.Shape.YChannel.Reference = "[5]/[2]"
oMyCurve.Shape.Line.Color.SetPredefinedColor(dd.eColorIndexBlue)
dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepPolarCurveListInt.htm`*

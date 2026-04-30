---
title: "IRepSpiderCurveListInt.Add"
description: "Generates a new curve in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveListInt.Add

!!! abstract "Method &middot; `ReportApi.chm`"
    Method: Add for SpiderCurves

Generates a new curve in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Add(ShapeType, Name)
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderShapeLine` | 0 | Line |
| `eSpiderShapeLineAndPoints` | 1 | Line and Points |

## Python example

```python
dd.Report.NewLayout()
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderAxisSystem")
oMyPos = oMyAxisSystem.Position.ByCoordinate
oMyPos.X1 = 20
oMyPos.X2 = 80
oMyPos.Y1 = 20
oMyPos.Y2 = 80

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLine, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/methods/Report_method_Add_IRepSpiderCurveListInt.htm`*

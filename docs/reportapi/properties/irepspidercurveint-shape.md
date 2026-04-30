---
title: "IRepSpiderCurveInt.Shape"
description: "Specifies the design of a curve in a spider axis system in DIAdem REPORT."
---

# IRepSpiderCurveInt.Shape

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Shape for SpiderCurve

Specifies the design of a curve in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Shape
```

## Python example

```python
dd.Data.Root.Clear()
dd.DataFileLoad("Example.tdm","TDM","")
dd.Report.NewLayout()

oMyAxisSystem = dd.Report.ActiveSheet.Objects.Add(dd.eReportObjectSpider, "MySpiderSystem")
oMySpiderCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMySpiderCurve.Shape.Channel.Reference = "[5]/[1]"

dd.MsgBoxDisp(oMySpiderCurve.ShapeType)
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Shape_IRepSpiderCurveInt.htm`*

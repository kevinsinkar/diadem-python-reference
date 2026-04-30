---
title: "IRepSpiderCurveInt.ShapeType"
description: "Specifies the display mode of a curve in a spider axis system in DIAdem REPORT. You can use the ChangeShape for SpiderCurves method to change the display mode."
---

# IRepSpiderCurveInt.ShapeType

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: ShapeType for SpiderCurve

Specifies the display mode of a curve in a spider axis system in DIAdem REPORT. You can use the ChangeShape for SpiderCurves method to change the display mode.

## Signature

```python
obj.ShapeType
```

## Enumeration values

| Name | Value | Description |
| --- | ---: | --- |
| `eSpiderShapeLine` | 0 | Line |
| `eSpiderShapeLineAndPoints` | 1 | Line and points |

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
<div class="SeeAlso"><h2>See Also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_ShapeType_IRepSpiderCurveInt.htm`*

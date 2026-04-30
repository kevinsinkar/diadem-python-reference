---
title: "IRepSpiderLabelAdditionalInt"
description: "The SpiderAdditionalLabel object provides the label properties of a curve in the Line and Points display type in DIAdem REPORT."
---

# IRepSpiderLabelAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderAdditionalLabel

The SpiderAdditionalLabel object provides the label properties of a curve in the Line and Points display type in DIAdem REPORT.

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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyAddLabel = oMyCurve.Shape.Extensions.Label
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.ValueVisible = True
oMyAddLabel.ValueFormat = "d"
oMyAddLabel.Angle = 90

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/irepspiderlabeladditionalint-angle/">Angle</a> | <a href="../../properties/irepspiderlabeladditionalint-font/">Font</a> | <a href="../../properties/irepspiderlabeladditionalint-relativeposition/">RelativePosition</a> | <a href="../../properties/irepspiderlabeladditionalint-separator/">Separator</a> | <a href="../../properties/irepspiderlabeladditionalint-text/">Text</a> | <a href="../../properties/irepspiderlabeladditionalint-textvisible/">TextVisible</a> | <a href="../../properties/irepspiderlabeladditionalint-usecurvecolor/">UseCurveColor</a> | <a href="../../properties/irepspiderlabeladditionalint-valueformat/">ValueFormat</a> | <a href="../../properties/irepspiderlabeladditionalint-valuevisible/">ValueVisible</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidershapeobjlineandpointsextensionsint/">SpiderLineAndPointsExtensions</a>.<a href="../../properties/irepspidershapeobjlineandpointsextensionsint-label/">Label</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderLabelAdditionalInt.htm`*

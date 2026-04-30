---
title: "IRepSpiderLabelNumericInt"
description: "The SpiderLabelNumeric object provides the font attributes of an axis scale in a spider axis system in DIAdem REPORT."
---

# IRepSpiderLabelNumericInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderLabelNumeric

The SpiderLabelNumeric object provides the font attributes of an axis scale in a spider axis system in DIAdem REPORT.

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

oMyAddLabel = oMyAxisSystem.CategorySettings.Axis.Numbers
oMyAddLabel.Font.Size = 1.5
oMyAddLabel.Format = "d"

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspiderlabelnumericint-font/">Font</a> | <a href="../../properties/irepspiderlabelnumericint-format/">Format</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspideraxisint/">SpiderAxis</a>.<a href="../../properties/irepspideraxisint-numbers/">Numbers</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderLabelNumericInt.htm`*

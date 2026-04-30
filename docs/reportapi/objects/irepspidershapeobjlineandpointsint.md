---
title: "IRepSpiderShapeObjLineAndPointsInt"
description: "The SpiderLineAndPoints object provides the curve properties of a spider axis system in the Line and points display mode in DIAdem REPORT."
---

# IRepSpiderShapeObjLineAndPointsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderLineAndPoints

The SpiderLineAndPoints object provides the curve properties of a spider axis system in the Line and points display mode in DIAdem REPORT.

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

oMySettings = oMyCurve.Shape.Settings
oMySettings.Line.LineType = dd.eLineTypeDashed2
oMySettings.Type = dd.eSpiderLineStaired
oMySettings.FillEffects.Color.ColorIndex = dd.eColorIndexYellow

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/irepspidershapeobjlineandpointsint-channel/">Channel</a> | <a href="../../properties/irepspidershapeobjlineandpointsint-extensions/">Extensions</a> | <a href="../../properties/irepspidershapeobjlineandpointsint-settings/">Settings</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidercurveint/">SpiderCurve</a>.<a href="../../properties/irepspidercurveint-shape/">Shape</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderShapeObjLineAndPointsInt.htm`*

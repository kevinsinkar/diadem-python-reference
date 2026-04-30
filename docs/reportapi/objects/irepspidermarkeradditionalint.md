---
title: "IRepSpiderMarkerAdditionalInt"
description: "The SpiderAdditionalMarker object provides the properties of the curve markers for a spider axis system in DIAdem REPORT."
---

# IRepSpiderMarkerAdditionalInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderAdditionalMarker

The SpiderAdditionalMarker object provides the properties of the curve markers for a spider axis system in DIAdem REPORT.

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

oMyMarker = oMyCurve.Shape.Extensions.Marker
oMyMarker.Type = dd.eMarkerSquare
oMyMarker.Size = 3
oMyMarker.Filling.UseCurveColor = True
oMyMarker.Line.Width = dd.eLineWidth0050

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties"><h2>Properties</h2>
<p><a href="../../properties/irepspidermarkeradditionalint-filling/">Filling</a> | <a href="../../properties/irepspidermarkeradditionalint-line/">Line</a> | <a href="../../properties/irepspidermarkeradditionalint-size/">Size</a> | <a href="../../properties/irepspidermarkeradditionalint-type/">Type</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidershapeobjlineandpointsextensionsint/">SpiderLineAndPointsExtensions</a>.<a href="../../properties/irepspidershapeobjlineandpointsextensionsint-marker/">Marker</a> | <a href="../irepspidershapeobjlineextensionsint/">SpiderLineExtensions</a>.<a href="../../properties/irepspidershapeobjlineextensionsint-marker/">Marker</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderMarkerAdditionalInt.htm`*

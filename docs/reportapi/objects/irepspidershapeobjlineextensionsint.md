---
title: "IRepSpiderShapeObjLineExtensionsInt"
description: "The SpiderLineExtensions object provides the extended curve properties of a spider axis system in the Line display mode in DIAdem REPORT."
---

# IRepSpiderShapeObjLineExtensionsInt

!!! abstract "Object &middot; `ReportApi.chm`"
    Object: SpiderLineExtensions

The SpiderLineExtensions object provides the extended curve properties of a spider axis system in the Line display mode in DIAdem REPORT.

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
oMyMarker.Filling.ColorIndex = dd.eColorIndexDarkGreen

dd.Report.Refresh()
```

## Members

<div markdown="1">
<div class="Properties">
<h2>Properties</h2>
<p><a href="../../properties/irepspidershapeobjlineextensionsint-marker/">Markers</a></p>
</div>
<div class="ReturnFrom"><h2>Returned From</h2>
<p><a href="../irepspidershapeobjlineint/">SpiderLine</a>.<a href="../../properties/irepspidershapeobjlineint-extensions/">Extensions</a></p>
</div>
</div>

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/Objects/Report_Objects_IRepSpiderShapeObjLineExtensionsInt.htm`*

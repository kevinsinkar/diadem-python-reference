---
title: "IRepSpiderShapeObjLineInt.Extensions"
description: "Specifies the extended properties of a curve in the Line display mode in a spider axis system in DIAdem REPORT."
---

# IRepSpiderShapeObjLineInt.Extensions

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Extensions for SpiderLine

Specifies the extended properties of a curve in the Line display mode in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Extensions
```

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

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Extensions_IRepSpiderShapeObjLineInt.htm`*

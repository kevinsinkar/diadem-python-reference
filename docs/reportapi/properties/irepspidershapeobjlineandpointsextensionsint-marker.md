---
title: "IRepSpiderShapeObjLineAndPointsExtensionsInt.Marker"
description: "Specifies the properties of the curve markers in the Line and points display mode in a spider axis system in DIAdem REPORT."
---

# IRepSpiderShapeObjLineAndPointsExtensionsInt.Marker

!!! abstract "Property &middot; `ReportApi.chm`"
    Property: Marker for SpiderLineAndPointsExtensions

Specifies the properties of the curve markers in the Line and points display mode in a spider axis system in DIAdem REPORT.

## Signature

```python
return_value = obj.Marker
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

oMyCurve = oMyAxisSystem.CurvesSpider.Add(dd.eSpiderShapeLineAndPoints, "MySpiderCurve")
oMyCurve.Shape.Channel.Reference = "[5]/[3]"

oMyMarker = oMyCurve.Shape.Extensions.Marker
oMyMarker.Line.Color.ColorIndex = dd.eColorIndexDarkYellow
oMyMarker.Type = dd.eMarkerCircle

dd.Report.Refresh()
```

## See also

<div markdown="1">
<div class="SeeAlso"><h2>See also</h2>
<p><a href="#" data-unresolved="1">Objects Overview</a></p>
</div>
</div>

---

*Source: `ReportApi/properties/Report_property_Marker_IRepSpiderShapeObjLineAndPointsExtensionsInt.htm`*
